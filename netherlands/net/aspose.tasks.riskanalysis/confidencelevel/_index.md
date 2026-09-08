---
title: "Enum ConfidenceLevel"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RiskAnalysis.ConfidenceLevel enum. Specificeert ondersteunde betrouwbaarheidsniveaus die worden gebruikt in risicoanalyse en die overeenkomen met het percentage van de tijd dat de werkelijke waarden binnen optimistische en pessimistische schattingen liggen."
type: docs
weight: 1850
url: /nl/net/aspose.tasks.riskanalysis/confidencelevel/
---
## ConfidenceLevel enumeration

Specificeert ondersteunde betrouwbaarheidsniveaus die in risicoanalyse worden gebruikt en overeenkomen met het percentage van de tijd dat de werkelijke waarden binnen optimistische en pessimistische schattingen vallen.

```csharp
public enum ConfidenceLevel
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| CL99 | `99` | 99 % Vertrouwensniveau. |
| CL95 | `95` | 95 % Vertrouwensniveau. |
| CL90 | `90` | 90 % Vertrouwensniveau. |
| CL85 | `85` | 85 % Vertrouwensniveau. |
| CL75 | `75` | 75 % Vertrouwensniveau. |

## Voorbeelden

Toont hoe risicoanalyse te starten met behulp van &lt;see cref="Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings" /&gt;.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Initialiseer een risicopatroon
var pattern = new RiskPattern(task)
{
    // Selecteer een distributietype voor de random‑getallengenerator om mogelijke waarden te genereren (momenteel worden slechts twee types ondersteund, namelijk normaal en uniform)            
    // Voor meer details zie hier: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Stel het percentage in van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario 
    // De standaardwaarde is 75, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de optimistische duur 3 dagen zal zijn.
    Optimistic = 70,

    // Stel het percentage in van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario 
    // De standaardwaarde is 125, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de pessimistische duur 5 dagen zal zijn.
    Pessimistic = 130,

    // Stel een betrouwbaarheidsniveau in dat overeenkomt met het percentage van de tijd dat de werkelijke waarden binnen de optimistische en pessimistische schattingen vallen. 
    // Je kunt het zien als een waarde van de standaarddeviatie: hoe onzekerder je bent over je schattingen, hoe hoger de waarde van de standaarddeviatie die in de random‑getallengenerator wordt gebruikt.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analyseer de projectrisico's
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

// instellingen wijzigen
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

### Zie ook

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


