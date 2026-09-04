---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API Reference"
description: "Führt eine Monte-Carlo-Simulation basierend auf den angegebenen Einstellungen der Risikoanalyse durch."
type: docs
weight: 264
url: /de/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Führt eine Monte-Carlo-Simulation basierend auf den angegebenen Einstellungen der Risikoanalyse durch.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Initialisiert eine neue Instanz der Klasse [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Führt eine Risikoanalyse für das angegebene Projekt durch. |
| [getSettings()](#getSettings--) | Ruft die Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) ab, die die erforderlichen Einstellungen für die Risikoanalyse definiert. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Setzt die Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings), die die erforderlichen Einstellungen für die Risikoanalyse definiert. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Initialisiert eine neue Instanz der Klasse [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | die angegebene Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Führt eine Risikoanalyse für das angegebene Projekt durch. Die Analyse basiert auf einer Monte‑Carlo‑Simulation und das Ergebnis ist eine Instanz der Klasse [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | die angegebene Instanz der Klasse [Project](../../com.aspose.tasks/project), die analysiert werden soll. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Ruft die Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) ab, die die erforderlichen Einstellungen für die Risikoanalyse definiert.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Setzt die Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings), die die erforderlichen Einstellungen für die Risikoanalyse definiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | die Instanz der Klasse [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings), die die erforderlichen Einstellungen für die Risikoanalyse definiert. |

