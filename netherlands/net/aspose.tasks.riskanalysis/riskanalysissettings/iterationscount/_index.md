---
title: "RiskAnalysisSettings.IterationsCount"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RiskAnalysisSettings eigenschap. Haalt het aantal iteraties op of stelt het in dat gebruikt wordt in Monte Carlo-simulatie. De standaardwaarde is 100"
type: docs
weight: 20
url: /nl/net/aspose.tasks.riskanalysis/riskanalysissettings/iterationscount/
---
## RiskAnalysisSettings.IterationsCount property

Haalt op of stelt het aantal iteraties in dat gebruikt wordt in Monte Carlo-simulatie. De standaardwaarde is 100.

```csharp
public int IterationsCount { get; set; }
```

## Voorbeelden

Toont hoe risicoanalyse‑instellingen voor Monte-Carlo-simulaties voor te bereiden.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Stel het aantal iteraties in voor Monte Carlo-simulatie (de standaardwaarde is 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Initialiseer een risicopatroon
var pattern = new RiskPattern(task);

// Selecteer een distributietype voor de random‑getallengenerator om mogelijke waarden te genereren (momenteel worden slechts twee types ondersteund, namelijk normaal en uniform)            
// Voor meer details zie hier: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Stel het percentage in van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario 
// De standaardwaarde is 75, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de optimistische duur 3 dagen zal zijn.
pattern.Optimistic = 70;

// Stel het percentage in van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario 
// De standaardwaarde is 125, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de pessimistische duur 5 dagen zal zijn.
pattern.Pessimistic = 130;

// Stel een betrouwbaarheidsniveau in dat overeenkomt met het percentage van de tijd dat de werkelijke waarden binnen de optimistische en pessimistische schattingen vallen. 
// Je kunt het zien als een waarde van de standaarddeviatie: hoe onzekerder je bent over je schattingen, hoe hoger de waarde van de standaarddeviatie die in de random‑getallengenerator wordt gebruikt.
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

### Zie ook

* class [RiskAnalysisSettings](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysissettings/)
* assembly [Aspose.Tasks](../../../)


