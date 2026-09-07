---
title: "RiskAnalyzer.Analyze"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "RiskAnalyzer metodo. Esegue l'analisi del rischio per il progetto specificato. L'analisi si basa su simulazione Monte Carlo e il risultato è un'istanza della classe RiskAnalysisResult."
type: docs
weight: 30
url: /it/net/aspose.tasks.riskanalysis/riskanalyzer/analyze/
---
## RiskAnalyzer.Analyze method

Esegue l'analisi del rischio per il progetto specificato. L'analisi si basa su simulazione Monte Carlo e il risultato è un'istanza della classe [`RiskAnalysisResult`](../../riskanalysisresult/).

```csharp
public RiskAnalysisResult Analyze(Project project)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | Project | l'istanza specificata della classe [`Project`](../../../aspose.tasks/project/) da analizzare. |

### Valore di ritorno

l'istanza della classe [`RiskAnalysisResult`](../../riskanalysisresult/) che rappresenta un risultato dell'analisi.

## Esempi

Mostra come avviare l'analisi dei rischi utilizzando &lt;see cref=\"Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings\" /&gt;.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// cambia impostazioni
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Vedi anche

* class [RiskAnalysisResult](../../riskanalysisresult/)
* class [Project](../../../aspose.tasks/project/)
* class [RiskAnalyzer](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalyzer/)
* assembly [Aspose.Tasks](../../../)


