---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Voert een Monte Carlo-simulatie uit op basis van de gespecificeerde instellingen voor risicoanalyse."
type: docs
weight: 264
url: /nl/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Voert een Monte Carlo-simulatie uit op basis van de gespecificeerde instellingen voor risicoanalyse.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Initialiseert een nieuwe instantie van de [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Voert risicoanalyse uit voor het opgegeven project. |
| [getSettings()](#getSettings--) | Haalt de instantie op van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse die de benodigde instellingen voor risicoanalyse definieert. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Stelt de instantie in van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse die de benodigde instellingen voor risicoanalyse definieert. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Initialiseert een nieuwe instantie van de [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | de opgegeven instantie van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse. |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Voert risicoanalyse uit voor het opgegeven project. De analyse is gebaseerd op Monte Carlo-simulatie en het resultaat is een instantie van de [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | de opgegeven instantie van de [Project](../../com.aspose.tasks/project) klasse om te analyseren. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Haalt de instantie op van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse die de benodigde instellingen voor risicoanalyse definieert.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Stelt de instantie in van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse die de benodigde instellingen voor risicoanalyse definieert.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | de instantie van de [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) klasse die de benodigde instellingen voor risicoanalyse definieert. |

