---
title: RiskAnalyzer
second_title: Aspose.Tasks for Java API Reference
description: Performs a Monte Carlo simulation based on the specified risk analysis settings.
type: docs
weight: 263
url: /java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Performs a Monte Carlo simulation based on the specified risk analysis settings.
## Constructors

| Constructor | Description |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Initializes a new instance of the [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) class. |
## Methods

| Method | Description |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Performs risk analysis for the specified project. |
| [getSettings()](#getSettings--) | Gets the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Sets the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Initializes a new instance of the [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | the specified instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class. |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Performs risk analysis for the specified project. The analysis is based on Monte Carlo simulation and the result is an instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | the specified instance of the [Project](../../com.aspose.tasks/project) class to analyze. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Gets the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Sets the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis. |

