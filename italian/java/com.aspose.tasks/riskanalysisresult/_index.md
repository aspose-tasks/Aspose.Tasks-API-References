---
title: "RiskAnalysisResult"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un risultato dell'analisi del rischio."
type: docs
weight: 262
url: /it/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Rappresenta un risultato dell'analisi del rischio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Restituisce un'istanza di [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) per il tipo di rischio specificato. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Salva il report di analisi del rischio nello stream in formato PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Salva il report di analisi del rischio nel percorso file specificato in formato PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Restituisce un'istanza di [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) per il tipo di rischio specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemType | int | il tipo di rischio specificato; può essere uno dei valori dell'enumerazione [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Salva il report di analisi del rischio nello stream in formato PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | java.io.InputStream | Lo stream su cui salvare il report di analisi del rischio. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Salva il report di analisi del rischio nel percorso file specificato in formato PDF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome file specificato. |

