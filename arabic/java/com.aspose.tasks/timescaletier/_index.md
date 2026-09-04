---
title: "TimescaleTier"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مستوى واحدًا من مقياس الوقت في مخطط جانت."
type: docs
weight: 325
url: /ar/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

يمثل مستوى واحدًا من مقياس الوقت في مخطط جانت.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | يُنشئ مثيلاً جديدًا من الفئة [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | يُنشئ مثيلاً جديدًا من الفئة [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAlignment()](#getAlignment--) | يحصل على طريقة محاذاة التسميات داخل كل فترة زمنية من المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | يحصل على الفاصل الزمني لوحدة الوقت الذي تُعرض فيه التسميات للمستوى. |
| [getDateTimeConverter()](#getDateTimeConverter--) | يحصل على دالة رد النداء لمعالجة رسم علامة التاريخ في هذا المستوى. |
| [getLabel()](#getLabel--) | يحصل على تسمية التاريخ [DateLabel](../../com.aspose.tasks/datelabel) للمستوى الزمني. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | يحصل على علم يحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. |
| [getShowTicks()](#getShowTicks--) | يحصل على قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى. |
| [getUnit()](#getUnit--) | يحصل على وحدة المقياس الزمني [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للمستوى الزمني. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | يحصل على قيمة تشير إلى ما إذا كان يجب اعتماد تسميات المستوى على السنة المالية. |
| [setAlignment(int value)](#setAlignment-int-) | يحدد طريقة محاذاة التسميات داخل كل فترة زمنية من المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | يحدد الفاصل الزمني لوحدة الوقت الذي تُعرض فيه التسميات للمستوى. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | يحدد دالة رد النداء لمعالجة رسم علامة التاريخ في هذا المستوى. |
| [setLabel(int value)](#setLabel-int-) | يحدد تسمية التاريخ [DateLabel](../../com.aspose.tasks/datelabel) للمستوى الزمني. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | يحدد علمًا يحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | يحدد قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى. |
| [setUnit(int value)](#setUnit-int-) | يحدد وحدة المقياس الزمني [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للمستوى الزمني. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | يحدد قيمة تشير إلى ما إذا كان يجب اعتماد تسميات المستوى على السنة المالية. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


يُنشئ مثيلاً جديدًا من الفئة [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


يُنشئ مثيلاً جديدًا من الفئة [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| unit | int | وحدة المقياس الزمني [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | عدد وحدات [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


يحصل على طريقة محاذاة التسميات داخل كل فترة زمنية من المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - طريقة محاذاة التسميات داخل كل فترة زمنية من المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


يحصل على الفاصل الزمني لوحدة الوقت الذي تُعرض فيه التسميات للمستوى. القيمة الافتراضية هي 1.

**Returns:**
int - الفاصل الزمني لوحدة الوقت الذي تُعرض فيه التسميات للمستوى.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


يحصل على دالة رد النداء لمعالجة رسم علامة التاريخ في هذا المستوى.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


يحصل على تسمية التاريخ [DateLabel](../../com.aspose.tasks/datelabel) للمستوى الزمني.

**Returns:**
int - تسمية التاريخ [DateLabel](../../com.aspose.tasks/datelabel) للمستوى الزمني.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


يحصل على علم يحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. إذا كانت القيمة 'true'، عندما تمتد الفترة على عدة صفحات، تُعرض تسميات التاريخ لتلك الفترة على كل صفحة. إذا كانت القيمة 'false'، تُعرض تسمية التاريخ مرة واحدة فقط وفقًا لقيمة `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\\#setAlignment-int-)) الخاصية.

--------------------

ليس له ما يعادله في MS Project.

**Returns:**
boolean - علامة تحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


يحصل على وحدة مقياس الزمن [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للطبقة الزمنية. القيمة الافتراضية هي [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - وحدة مقياس الزمن [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للطبقة الزمنية.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


يحصل على قيمة تشير إلى ما إذا كان يجب اعتماد تسميات المستوى على السنة المالية.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان يجب أن تستند تسميات المستوى إلى السنة المالية.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


يحدد طريقة محاذاة التسميات داخل كل فترة زمنية من المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | كيفية محاذاة التسميات داخل كل فترة زمنية في المستوى ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


يضبط الفاصل الزمني لوحدة الوقت التي تُظهر فيها التسميات للمستوى. القيمة الافتراضية هي 1.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | الفاصل الزمني لوحدة الوقت التي تُظهر فيها التسميات للمستوى. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


يحدد دالة رد النداء لمعالجة رسم علامة التاريخ في هذا المستوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | دالة رد نداء لمعالجة رسم علامة التاريخ في هذا المستوى. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


يحدد تسمية التاريخ [DateLabel](../../com.aspose.tasks/datelabel) للمستوى الزمني.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | تسمية تاريخ [DateLabel](../../com.aspose.tasks/datelabel) للطبقة الزمنية. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


يضبط العلامة التي تحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. إذا كانت القيمة 'true'، عندما تمتد الفترة الزمنية على عدة صفحات، تُعرض تسميات التاريخ للفترة على كل صفحة. إذا كانت القيمة 'false'، تُعرض تسمية التاريخ مرة واحدة فقط وفقًا لقيمة `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) الخاصية.

--------------------

ليس له ما يعادله في MS Project.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | علامة تحدد ما إذا كان يجب عرض تسميات التاريخ على كل صفحة عندما تمتد فترة زمنية على عدة صفحات. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


يحدد قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب إظهار علامات الفواصل التي تفصل الفترات الزمنية في المستوى. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


يضبط وحدة مقياس الزمن [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للطبقة الزمنية. القيمة الافتراضية هي [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | وحدة مقياس الزمن [TimescaleUnit](../../com.aspose.tasks/timescaleunit) للطبقة الزمنية. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


يحدد قيمة تشير إلى ما إذا كان يجب اعتماد تسميات المستوى على السنة المالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان يجب أن تستند تسميات المستوى إلى السنة المالية. |

