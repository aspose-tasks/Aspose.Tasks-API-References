---
title: "RiskAnalysisResult"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un resultado de análisis de riesgos."
type: docs
weight: 262
url: /es/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Representa un resultado de análisis de riesgos.
## Métodos

| Método | Descripción |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Devuelve una instancia de [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) para el tipo de riesgo especificado. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Guarda el informe de análisis de riesgos en el flujo en formato PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Guarda el informe de análisis de riesgos en la ruta de archivo especificada en formato PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Devuelve una instancia de [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) para el tipo de riesgo especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| itemType | int | el tipo de riesgo especificado; puede ser uno de los valores de la enumeración [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Guarda el informe de análisis de riesgos en el flujo en formato PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | java.io.InputStream | El flujo donde guardar el informe de análisis de riesgos. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Guarda el informe de análisis de riesgos en la ruta de archivo especificada en formato PDF.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre de archivo especificado. |

