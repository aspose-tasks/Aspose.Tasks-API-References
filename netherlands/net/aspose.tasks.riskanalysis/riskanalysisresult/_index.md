---
title: "Klasse RiskAnalysisResult"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalysisResult klasse. Vertegenwoordigt een resultaat van risicoanalyse."
type: docs
weight: 1870
url: /nl/net/aspose.tasks.riskanalysis/riskanalysisresult/
---
## RiskAnalysisResult class

Stelt een resultaat van risicoanalyse voor.

```csharp
public class RiskAnalysisResult
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetRiskItems](../../aspose.tasks.riskanalysis/riskanalysisresult/getriskitems/)(RiskItemType) | Retourneert een instantie van de [`RiskItemStatisticsCollection`](../riskitemstatisticscollection/) voor het opgegeven risico-type. |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport)(Stream) | Slaat het risicoanalyse‑rapport op in de stream in PDF-formaat. |
| [SaveReport](../../aspose.tasks.riskanalysis/riskanalysisresult/savereport/#savereport_1)(string) | Slaat het risicoanalyse‑rapport op naar het opgegeven bestandspad in PDF-formaat. |

## Voorbeelden

Toont hoe statistieken van risico's te berekenen en deze op te slaan als PDF‑rapport.

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

// sla analyse op als rapport in een bestand via bestandspad
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// of sla analyse op in een stream
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Zie ook

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


