---
title: "RiskItemStatistics"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل عنصرًا يخزن البيانات الإحصائية للمهمة في المشروع المُحلَّل."
type: docs
weight: 265
url: /ar/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

يمثل عنصرًا يخزن البيانات الإحصائية للمهمة في المشروع المُحلَّل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | يحصل على القيمة المتوقعة لعنصر المخاطر. |
| [getItemType()](#getItemType--) | يحصل على نسخة من تعداد [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | يحصل على القيمة القصوى التي تم توليدها أثناء محاكاة مونت كارلو. |
| [getMinimum()](#getMinimum--) | يحصل على القيمة الدنيا التي تم توليدها أثناء محاكاة مونت كارلو. |
| [getPercentile(int percent)](#getPercentile-int-) | يحصل على قيمة يكون أقل منها نسبة مئوية محددة من العينات المولدة. |
| [getStandardDeviation()](#getStandardDeviation--) | يحصل على الانحراف المعياري لعنصر المخاطر. |
| [toString()](#toString--) | يرجع تمثيلًا نصيًا قصيرًا لعنصر المخاطر. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


يحصل على القيمة المتوقعة لعنصر المخاطر.

**Returns:**
java.util.Date - القيمة المتوقعة لعنصر المخاطر.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


يحصل على نسخة من تعداد [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - مثال على تعداد [RiskItemType](../../com.aspose/tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


يحصل على القيمة القصوى التي تم توليدها أثناء محاكاة مونت كارلو.

**Returns:**
java.util.Date - القيمة القصوى التي تم توليدها خلال محاكاة مونت كارلو.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


يحصل على القيمة الدنيا التي تم توليدها أثناء محاكاة مونت كارلو.

**Returns:**
java.util.Date - القيمة الدنيا التي تم توليدها خلال محاكاة مونت كارلو.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


يحصل على قيمة يكون أقل منها نسبة مئوية محددة من العينات المولدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| النسبة المئوية | int | النسبة المحددة بين 0 و 100. |

**Returns:**
java.util.Date - قيمة يكون أقل منها نسبة مئوية محددة من العينات المولدة.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


يحصل على الانحراف المعياري لعنصر المخاطر.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


يعيد تمثيلًا نصيًا قصيرًا لعنصر المخاطر. التفاصيل الدقيقة للتمثيل غير محددة وقابلة للتغيير.

**Returns:**
java.lang.String - نص قصير يمثل كائن RiskItem.
