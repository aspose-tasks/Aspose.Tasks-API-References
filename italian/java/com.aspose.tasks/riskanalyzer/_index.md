---
title: "RiskAnalyzer"
second_title: "Aspose.Tasks for Java API Reference"
description: "Esegue una simulazione Monte Carlo basata sulle impostazioni di analisi del rischio specificate."
type: docs
weight: 264
url: /it/java/com.aspose.tasks/riskanalyzer/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalyzer
```

Esegue una simulazione Monte Carlo basata sulle impostazioni di analisi del rischio specificate.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RiskAnalyzer(RiskAnalysisSettings settings)](#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-) | Inizializza una nuova istanza della classe [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [analyze(Project project)](#analyze-com.aspose.tasks.Project-) | Esegue l'analisi del rischio per il progetto specificato. |
| [getSettings()](#getSettings--) | Ottiene l'istanza della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) che definisce le impostazioni necessarie per l'analisi del rischio. |
| [setSettings(RiskAnalysisSettings value)](#setSettings-com.aspose.tasks.RiskAnalysisSettings-) | Imposta l'istanza della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) che definisce le impostazioni necessarie per l'analisi del rischio. |
### RiskAnalyzer(RiskAnalysisSettings settings) {#RiskAnalyzer-com.aspose.tasks.RiskAnalysisSettings-}
```
public RiskAnalyzer(RiskAnalysisSettings settings)
```


Inizializza una nuova istanza della classe [RiskAnalyzer](../../com.aspose.tasks/riskanalyzer).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | l'istanza specificata della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings). |

### analyze(Project project) {#analyze-com.aspose.tasks.Project-}
```
public final RiskAnalysisResult analyze(Project project)
```


Esegue l'analisi del rischio per il progetto specificato. L'analisi si basa sulla simulazione Monte Carlo e il risultato è un'istanza della classe [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | l'istanza specificata della classe [Project](../../com.aspose.tasks/project) da analizzare. |

**Returns:**
[RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) - the instance of the [RiskAnalysisResult](../../com.aspose.tasks/riskanalysisresult) which represents a result of the analysis.
### getSettings() {#getSettings--}
```
public final RiskAnalysisSettings getSettings()
```


Ottiene l'istanza della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) che definisce le impostazioni necessarie per l'analisi del rischio.

**Returns:**
[RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) - the instance of the [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) class which defines necessary settings for risk analysis.
### setSettings(RiskAnalysisSettings value) {#setSettings-com.aspose.tasks.RiskAnalysisSettings-}
```
public final void setSettings(RiskAnalysisSettings value)
```


Imposta l'istanza della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) che definisce le impostazioni necessarie per l'analisi del rischio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) | l'istanza della classe [RiskAnalysisSettings](../../com.aspose.tasks/riskanalysissettings) che definisce le impostazioni necessarie per l'analisi del rischio. |

