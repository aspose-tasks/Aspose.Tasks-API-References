---
title: "المعدل"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل تعريف فترة زمنية والأسعار المطبقة على مورد خلال تلك الفترة."
type: docs
weight: 232
url: /ar/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

يمثل تعريف فترة زمنية والأسعار المطبقة على مورد خلال تلك الفترة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | يحصل على التكلفة لكل استخدام لمورد. |
| [getOvertimeRate()](#getOvertimeRate--) | يحصل على معدل العمل الإضافي لكل ساعة لمورد. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | يحصل على الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي. |
| [getRateTable()](#getRateTable--) | يحصل على المعرف الفريد لجدول المعدلات لمورد. |
| [getRatesFrom()](#getRatesFrom--) | يحصل على التاريخ الذي يصبح فيه المعدل ساريًا. |
| [getRatesTo()](#getRatesTo--) | يحصل على آخر تاريخ يكون فيه المعدل ساريًا. |
| [getStandardRate()](#getStandardRate--) | يحصل على المعدل القياسي لكل ساعة لمورد. |
| [getStandardRateFormat()](#getStandardRateFormat--) | يحصل على الوحدات التي يستخدمها Microsoft Project لعرض المعدل القياسي. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | يحدد تكلفة الاستخدام لكل مورد. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | يحدد معدل العمل الإضافي لكل ساعة لمورد. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | يحدد الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي. |
| [setRateTable(int value)](#setRateTable-int-) | يحدد المعرف الفريد لجدول الأسعار لمورد. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | يحدد التاريخ الذي يصبح فيه السعر ساريًا. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | يحدد آخر تاريخ يكون فيه السعر ساريًا. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | يحدد السعر القياسي لكل ساعة لمورد. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | يحدد الوحدات التي يستخدمها Microsoft Project لعرض السعر القياسي. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


يحصل على تكلفة الاستخدام لكل مورد. يتم استرجاع هذه القيمة من التاريخ الحالي إذا كان هناك جدول أسعار للمورد.

**Returns:**
java.math.BigDecimal - تكلفة الاستخدام لكل مورد.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


يحصل على معدل العمل الإضافي لكل ساعة لمورد.

**Returns:**
java.math.BigDecimal - معدل العمل الإضافي لكل ساعة لمورد.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


يحصل على الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي.

**Returns:**
int - الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


يحصل على المعرف الفريد لجدول المعدلات لمورد.

**Returns:**
int - المعرف الفريد لجدول الأسعار لمورد.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


يحصل على التاريخ الذي يصبح فيه المعدل ساريًا.

**Returns:**
java.util.Date - التاريخ الذي يصبح فيه السعر ساريًا.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


يحصل على آخر تاريخ يكون فيه المعدل ساريًا.

**Returns:**
java.util.Date - آخر تاريخ يكون فيه السعر ساريًا.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


يحصل على المعدل القياسي لكل ساعة لمورد.

**Returns:**
java.math.BigDecimal - السعر القياسي لكل ساعة لمورد.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


يحصل على الوحدات التي يستخدمها Microsoft Project لعرض المعدل القياسي.

**Returns:**
int - الوحدات التي يستخدمها Microsoft Project لعرض السعر القياسي.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


يحدد تكلفة الاستخدام لكل مورد. يتم استرجاع هذه القيمة من التاريخ الحالي إذا كان هناك جدول أسعار للمورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | تكلفة الاستخدام لكل مورد. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


يحدد معدل العمل الإضافي لكل ساعة لمورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | معدل العمل الإضافي لكل ساعة لمورد. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


يحدد الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


يحدد المعرف الفريد لجدول الأسعار لمورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعرف الفريد لجدول الأسعار لمورد. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


يحدد التاريخ الذي يصبح فيه السعر ساريًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | التاريخ الذي يصبح فيه السعر ساريًا. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


يحدد آخر تاريخ يكون فيه السعر ساريًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | آخر تاريخ يكون فيه السعر ساريًا. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


يحدد السعر القياسي لكل ساعة لمورد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | السعر القياسي لكل ساعة لمورد. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


يحدد الوحدات التي يستخدمها Microsoft Project لعرض السعر القياسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الوحدات المستخدمة من قبل Microsoft Project لعرض السعر القياسي. |

