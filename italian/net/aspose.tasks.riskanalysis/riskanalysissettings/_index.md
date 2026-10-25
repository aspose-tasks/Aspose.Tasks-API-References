---
title: "Classe RiskAnalysisSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings. Specifica le impostazioni per eseguire l'analisi del rischio"
type: docs
weight: 1880
url: /it/net/aspose.tasks.riskanalysis/riskanalysissettings/
---
## RiskAnalysisSettings class

Specifica le impostazioni per eseguire l'analisi del rischio.

```csharp
public class RiskAnalysisSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RiskAnalysisSettings](riskanalysissettings/)() | Inizializza una nuova istanza della classe `RiskAnalysisSettings`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IterationsCount](../../aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/) { get; set; } | Ottiene o imposta il numero di iterazioni da utilizzare nella simulazione Monte Carlo. Il valore predefinito è 100. |
| [Patterns](../../aspose.tasks.riskanalysis/riskanalysissettings/patterns/) { get; } | Ottiene una collezione contenente le istanze della classe [`RiskPattern`](../riskpattern/). |

## Esempi

Mostra come preparare le impostazioni di analisi del rischio per le simulazioni Monte Carlo.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Imposta il numero di iterazioni per la simulazione Monte Carlo (il valore predefinito è 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inizializza un modello di rischio
var pattern = new RiskPattern(task);

// Seleziona un tipo di distribuzione per il generatore di numeri casuali da cui generare valori possibili (attualmente sono supportati solo due tipi, ovvero normale e uniforme)
// Per ulteriori dettagli vedi qui: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore
// Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni
pattern.Optimistic = 70;

// Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore
// Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni.
pattern.Pessimistic = 130;

// Imposta un livello di confidenza che corrisponde alla percentuale di tempo in cui i valori reali saranno compresi tra le stime ottimistiche e pessimistiche.
// Puoi considerarlo come un valore di deviazione standard: più sei incerto sulle tue stime, più il valore di deviazione standard usato nel generatore di numeri casuali sarà elevato.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Vedi anche

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


