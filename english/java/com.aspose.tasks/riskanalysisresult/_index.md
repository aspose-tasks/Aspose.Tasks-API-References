---
title: RiskAnalysisResult
second_title: Aspose.Tasks for Java API Reference
description: Represents a result of risk analysis.
type: docs
weight: 261
url: /java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

Represents a result of risk analysis.
## Methods

| Method | Description |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | Returns an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | Saves the risk analysis report to the stream in PDF format. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Saves the risk analysis report to the specified file path in PDF format. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


Returns an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemType | int | the specified risk type; can be one of the values of the [RiskItemType](../../com.aspose.tasks/riskitemtype) enumeration. |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


Saves the risk analysis report to the stream in PDF format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream to save risk analysis report to. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the risk analysis report to the specified file path in PDF format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The specified file name. |

