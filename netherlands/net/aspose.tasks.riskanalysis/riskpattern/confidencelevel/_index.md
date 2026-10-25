---
title: "RiskPattern.ConfidenceLevel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RiskPattern eigenschap. Haalt of stelt het vertrouwensniveau in dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen vallen. De standaardwaarde is CL99"
type: docs
weight: 20
url: /nl/net/aspose.tasks.riskanalysis/riskpattern/confidencelevel/
---
## RiskPattern.ConfidenceLevel property

Haalt of stelt het betrouwbaarheidsniveau in dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen de optimistische en pessimistische schattingen zullen liggen. De standaardwaarde is CL99.

```csharp
public ConfidenceLevel ConfidenceLevel { get; set; }
```

## Opmerkingen

Kan een van de waarden zijn die zijn gedefinieerd in de `ConfidenceLevel`-enumeratie.

## Voorbeelden

Toont hoe risicosimulatie-instellingen te definiëren.

```csharp
var settings = new RiskAnalysisSettings();
settings.IterationsCount = 200;

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

### Zie ook

* enum [ConfidenceLevel](../../confidencelevel/)
* class [RiskPattern](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpattern/)
* assembly [Aspose.Tasks](../../../)


