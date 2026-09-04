---
title: "RiskAnalyzer"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Effectue une simulation Monte Carlo basée sur les paramètres d'analyse de risque spécifiés."
type: docs
weight: 264
url: /fr/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Effectue une simulation Monte Carlo basée sur les paramètres d'analyse de risque spécifiés.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Initialise une nouvelle instance de la classe [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Effectue une analyse de risque pour le projet spécifié. |
| [getSettings()](#getSettings--) | Obtient l'instance de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) qui définit les paramètres nécessaires à l'analyse de risque. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Définit l'instance de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) qui définit les paramètres nécessaires à l'analyse de risque. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Initialise une nouvelle instance de la classe [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | l'instance spécifiée de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Effectue une analyse de risque pour le projet spécifié. L'analyse est basée sur une simulation Monte Carlo et le résultat est une instance de la classe [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | l'instance spécifiée de la classe [Project](../../com.aspose.tasks/project) à analyser. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Obtient l'instance de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) qui définit les paramètres nécessaires à l'analyse de risque.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Définit l'instance de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) qui définit les paramètres nécessaires à l'analyse de risque.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | l'instance de la classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) qui définit les paramètres nécessaires à l'analyse de risque. |

