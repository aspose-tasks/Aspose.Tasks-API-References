---
title: "RiskAnalyzer.Analyze"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RiskAnalyzer methode. Voert risicoanalyse uit voor het opgegeven project. De analyse is gebaseerd op Monte Carlo-simulatie en het resultaat is een instantie van de RiskAnalysisResult-klasse."
type: docs
weight: 30
url: /nl/net/aspose.tasks.riskanalysis/riskanalyzer/analyze/
---
## RiskAnalyzer.Analyze method

Voert risicoanalyse uit voor het opgegeven project. De analyse is gebaseerd op Monte Carlo-simulatie en het resultaat is een instantie van de [`RiskAnalysisResult`](../../riskanalysisresult/) klasse.

```csharp
public RiskAnalysisResult Analyze(Project project)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | de opgegeven instantie van de [`Project`](../../../aspose.tasks/project/) klasse om te analyseren. |

### Retourwaarde

de instantie van de [`RiskAnalysisResult`](../../riskanalysisresult/) die een resultaat van de analyse vertegenwoordigt.

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

* class [RiskAnalysisResult](../../riskanalysisresult/)
* class [Project](../../../aspose.tasks/project/)
* class [RiskAnalyzer](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalyzer/)
* assembly [Aspose.Tasks](../../../)


