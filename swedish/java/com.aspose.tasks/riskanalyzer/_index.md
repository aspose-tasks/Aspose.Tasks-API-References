---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API-referens"
description: "Utför en Monte Carlo-simulering baserad på de angivna riskanalysinställningarna."
type: docs
weight: 264
url: /sv/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Utför en Monte Carlo-simulering baserad på de angivna riskanalysinställningarna.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Initierar en ny instans av klassen [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Utför riskanalys för det angivna projektet. |
| [getSettings()](#getSettings--) | Hämtar instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) som definierar nödvändiga inställningar för riskanalys. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Ställer in instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) som definierar nödvändiga inställningar för riskanalys. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Initierar en ny instans av klassen [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | den angivna instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Utför riskanalys för det angivna projektet. Analysen baseras på Monte Carlo-simulering och resultatet är en instans av klassen [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | den angivna instansen av klassen [Project](../../com.aspose.tasks/project) att analysera. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Hämtar instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) som definierar nödvändiga inställningar för riskanalys.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Ställer in instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) som definierar nödvändiga inställningar för riskanalys.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | instansen av klassen [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) som definierar nödvändiga inställningar för riskanalys. |

