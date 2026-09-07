---
title: "RiskPattern.Distribution"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "RiskPattern proprietà. Ottiene o imposta la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. Il valore predefinito è ProbabilityDistributionType.Normal"
type: docs
weight: 30
url: /it/net/aspose.tasks.riskanalysis/riskpattern/distribution/
---
## RiskPattern.Distribution property

Ottiene o imposta la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. Il valore predefinito è ProbabilityDistributionType.Normal.

```csharp
public ProbabilityDistributionType Distribution { get; set; }
```

## Osservazioni

Può essere uno dei valori definiti nell'enumerazione [`ProbabilityDistributionType`](../../probabilitydistributiontype/).

## Esempi

Mostra come definire le impostazioni di simulazione del rischio.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

settings.Patterns.Add(pattern);

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

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Vedi anche

* enum [ProbabilityDistributionType](../../probabilitydistributiontype/)
* class [RiskPattern](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpattern/)
* assembly [Aspose.Tasks](../../../)


