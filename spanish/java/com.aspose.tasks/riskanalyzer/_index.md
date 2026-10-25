---
title: "RiskAnalyzer"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Realiza una simulación Monte Carlo basada en la configuración de análisis de riesgos especificada."
type: docs
weight: 264
url: /es/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Realiza una simulación Monte Carlo basada en la configuración de análisis de riesgos especificada.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Inicializa una nueva instancia de la clase [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer). |
## Métodos

| Método | Descripción |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Realiza un análisis de riesgos para el proyecto especificado. |
| [getSettings()](#getSettings--) | Obtiene la instancia de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) que define la configuración necesaria para el análisis de riesgos. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Establece la instancia de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) que define la configuración necesaria para el análisis de riesgos. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Inicializa una nueva instancia de la clase [RiskAnalyzer](../../com.aspose/tasks/riskanalyzer).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | la instancia especificada de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Realiza un análisis de riesgos para el proyecto especificado. El análisis se basa en una simulación de Monte Carlo y el resultado es una instancia de la clase [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | la instancia especificada de la clase [Project](../../com.aspose.tasks/project) para analizar. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Obtiene la instancia de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) que define la configuración necesaria para el análisis de riesgos.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Establece la instancia de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) que define la configuración necesaria para el análisis de riesgos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | la instancia de la clase [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) que define la configuración necesaria para el análisis de riesgos. |

