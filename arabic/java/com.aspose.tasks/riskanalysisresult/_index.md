---
title: "RiskAnalysisResult"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل نتيجة تحليل المخاطر."
type: docs
weight: 262
url: /ar/java/com.aspose.tasks/riskanalysisresult/
---

**Inheritance:**
java.lang.Object
```
public class RiskAnalysisResult
```

يمثل نتيجة تحليل المخاطر.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getRiskItems(int itemType)](#getRiskItems-int-) | إرجاع مثيل من [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) لنوع المخاطر المحدد. |
| [saveReport(InputStream stream)](#saveReport-java.io.InputStream-) | يحفظ تقرير تحليل المخاطر إلى الدفق بتنسيق PDF. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | يحفظ تقرير تحليل المخاطر إلى مسار الملف المحدد بتنسيق PDF. |
### getRiskItems(int itemType) {#getRiskItems-int-}
```
public final RiskItemStatisticsCollection getRiskItems(int itemType)
```


إرجاع مثيل من [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) لنوع المخاطر المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| itemType | int | نوع المخاطر المحدد؛ يمكن أن يكون أحد قيم تعداد [RiskItemType](../../com.aspose.tasks/riskitemtype). |

**Returns:**
[RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) - an instance of the [RiskItemStatisticsCollection](../../com.aspose.tasks/riskitemstatisticscollection) for the specified risk type.
### saveReport(InputStream stream) {#saveReport-java.io.InputStream-}
```
public final void saveReport(InputStream stream)
```


يحفظ تقرير تحليل المخاطر إلى الدفق بتنسيق PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stream | java.io.InputStream | الدفق لحفظ تقرير تحليل المخاطر إليه. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


يحفظ تقرير تحليل المخاطر إلى مسار الملف المحدد بتنسيق PDF.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف المحدد. |

