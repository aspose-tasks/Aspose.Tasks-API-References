---
title: "Classe RiskItemStatistics"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RiskAnalysis.RiskItemStatistics. Rappresenta un elemento che memorizza dati statistici per l'attività del progetto analizzato."
type: docs
weight: 1900
url: /it/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Rappresenta un elemento che memorizza i dati statistici per l'attività del progetto analizzato.

```csharp
public class RiskItemStatistics
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Restituisce il valore atteso dell'elemento di rischio. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | Restituisce un'istanza dell'enumerazione [`RiskItemType`](../riskitemtype/). |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Restituisce il valore massimo generato durante la simulazione Monte Carlo. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Restituisce il valore minimo generato durante la simulazione Monte Carlo. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Restituisce la deviazione standard dell'elemento di rischio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Restituisce un valore al di sotto del quale cade una percentuale specificata di campioni generati. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Restituisce una breve rappresentazione testuale di un elemento di rischio. I dettagli esatti della rappresentazione non sono specificati e possono cambiare. |

## Esempi

Mostra come calcolare le statistiche dei rischi.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inizializza un modello di rischio
var pattern = new RiskPattern(task)
{
    // Seleziona un tipo di distribuzione per il generatore di numeri casuali da cui generare valori possibili (attualmente sono supportati solo due tipi, ovvero normale e uniforme)
    // Per ulteriori dettagli vedi qui: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore
    // Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni
    Optimistic = 70,

    // Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore
    // Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni.
    Pessimistic = 130,

    // Imposta un livello di confidenza che corrisponde alla percentuale di tempo in cui i valori reali saranno compresi tra le stime ottimistiche e pessimistiche.
    // Puoi considerarlo come un valore di deviazione standard: più sei incerto sulle tue stime, più il valore di deviazione standard usato nel generatore di numeri casuali sarà elevato.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analizza i rischi del progetto
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### Vedi anche

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


