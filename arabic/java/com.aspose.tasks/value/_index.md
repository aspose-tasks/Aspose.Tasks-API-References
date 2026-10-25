---
title: "القيمة"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل قيمة في قائمة القيم."
type: docs
weight: 333
url: /ar/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

يمثل قيمة في قائمة القيم.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Value()](#Value--) | ينشئ مثلاً جديدًا من الفئة [Value](../../com.aspose/tasks/value). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDateValue()](#getDateValue--) | يحصل على القيمة الفعلية إذا كان يمكن تمثيلها كـ DateTime. |
| [getDescription()](#getDescription--) | يحصل على وصف القيمة. |
| [getDuration()](#getDuration--) | يحصل على القيمة الفعلية المستخدمة لتمثيل المدة. |
| [getId()](#getId--) | يحصل على المعرف الفريد للقيمة عبر المشروع. |
| [getNumericValue()](#getNumericValue--) | يحصل على القيمة الفعلية المستخدمة لتمثيل العدد أو قيمة التكلفة. |
| [getPhonetic()](#getPhonetic--) | يحصل على المعلومات الصوتية حول اسم الحقل المخصص. |
| [getStringValue()](#getStringValue--) | يحصل على القيمة الفعلية المستخدمة لتمثيل سلسلة النص. |
| [getVal()](#getVal--) | يحصل على القيمة الفعلية في التمثيل الداخلي. |
| [getValueGuid()](#getValueGuid--) | يحصل على GUID يحدد هذه القيمة بين الآخرين في المشروع بأكمله. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | يضبط القيمة الفعلية إذا كان يمكن تمثيلها كـ DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | يضبط وصف القيمة. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | يضبط القيمة الفعلية المستخدمة لتمثيل المدة. |
| [setId(int value)](#setId-int-) | يضبط المعرف الفريد للقيمة عبر المشروع. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | يضبط القيمة الفعلية المستخدمة لتمثيل العدد أو قيمة التكلفة. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | يضبط المعلومات الصوتية حول اسم الحقل المخصص. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | يضبط القيمة الفعلية المستخدمة لتمثيل سلسلة النص. |
| [setVal(String value)](#setVal-java.lang.String-) | يضبط القيمة الفعلية في التمثيل الداخلي. |
### Value() {#Value--}
```
public Value()
```


ينشئ مثلاً جديدًا من الفئة [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


يحصل على القيمة الفعلية إذا كان يمكن تمثيلها كـ DateTime. القيمة الافتراضية هي DateTime\#MinValue.MinValue.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة DateTime.

**Returns:**
java.util.Date - القيمة الفعلية إذا يمكن تمثيلها كـ DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


يحصل على وصف القيمة.

**Returns:**
java.lang.String - وصف القيمة.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


يحصل على القيمة الفعلية المستخدمة لتمثيل المدة.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


يحصل على المعرف الفريد للقيمة عبر المشروع.

من المهم عدم وجود معرفات متطابقة لمثيلات [Value](../../com.aspose.tasks/value) المختلفة.

القيمة الدنيا لـ `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) هي `1`.

**Returns:**
int - المعرف الفريد لقيمة عبر المشروع.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


يحصل على القيمة الفعلية المستخدمة لتمثيل العدد أو قيمة التكلفة.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Number أو Cost.

**Returns:**
java.math.BigDecimal - القيمة الفعلية المستخدمة لتمثيل قيمة رقم أو تكلفة.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


يحصل على المعلومات الصوتية حول اسم الحقل المخصص.

**Returns:**
java.lang.String - المعلومات الصوتية حول اسم الحقل المخصص.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


يحصل على القيمة الفعلية المستخدمة لتمثيل سلسلة النص.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Text.

**Returns:**
java.lang.String - القيمة الفعلية المستخدمة لتمثيل سلسلة نصية.
### getVal() {#getVal--}
```
public final String getVal()
```


يحصل على القيمة الفعلية في التمثيل الداخلي. يفضل استخدام الخصائص ذات النوع القوي المذكورة أدناه.

--------------------

إذا كنت تريد تعيين قيمة Text، يفضل استخدام الخاصية ذات النوع القوي `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

إذا كنت تريد تعيين قيمة Number أو Cost، يفضل استخدام الخاصية ذات النوع القوي `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

إذا كنت تريد تعيين قيم Date/Start/Finish، يفضل استخدام الخاصية ذات النوع القوي `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

إذا كنت تريد تعيين قيمة Duration، يفضل استخدام الخاصية ذات النوع القوي `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

إذا لم يكن نوعك مدرجًا، استخدم الخاصية `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Returns:**
java.lang.String - القيمة الفعلية في التمثيل الداخلي.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


يحصل على GUID يحدد هذه القيمة بين الآخرين في المشروع بأكمله.

**Returns:**
java.util.UUID - معرف GUID يحدد هذه القيمة بين القيم الأخرى في المشروع بأكمله.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


يضبط القيمة الفعلية إذا يمكن تمثيلها كـ DateTime. القيمة الافتراضية هي DateTime\#MinValue.MinValue.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة DateTime.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | القيمة الفعلية إذا يمكن تمثيلها كـ DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


يضبط وصف القيمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | وصف القيمة. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


يضبط القيمة الفعلية المستخدمة لتمثيل المدة.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Duration.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | القيمة الفعلية المستخدمة لتمثيل Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


يضبط المعرف الفريد للقيمة عبر المشروع.

من المهم عدم وجود معرفات متطابقة لمثيلات [Value](../../com.aspose.tasks/value) المختلفة.

القيمة الدنيا لـ `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) هي `1`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعرّف الفريد لقيمة عبر المشروع. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


يضبط القيمة الفعلية المستخدمة لتمثيل العدد أو قيمة التكلفة.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Number أو Cost.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | القيمة الفعلية المستخدمة لتمثيل الرقم أو قيمة التكلفة. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


يضبط المعلومات الصوتية حول اسم الحقل المخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | المعلومات الصوتية حول اسم الحقل المخصص. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


يضبط القيمة الفعلية المستخدمة لتمثيل سلسلة النص.

--------------------

يفضل استخدام هذه الخاصية بدلاً من `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), عندما تحتاج إلى تعيين قيمة Text.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة الفعلية المستخدمة لتمثيل سلسلة النص. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


يضبط القيمة الفعلية في التمثيل الداخلي. يفضّل استخدام الخصائص ذات النوع القوي المذكورة أدناه.

--------------------

إذا كنت تريد تعيين قيمة Text، يفضل استخدام الخاصية ذات النوع القوي `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

إذا كنت تريد تعيين قيمة Number أو Cost، يفضل استخدام الخاصية ذات النوع القوي `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

إذا كنت تريد ضبط قيم Date/Start/Finish، يفضّل استخدام الخاصية ذات النوع القوي `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) property.

إذا كنت تريد تعيين قيمة Duration، يفضل استخدام الخاصية ذات النوع القوي `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

إذا لم يكن نوعك مدرجًا، استخدم الخاصية `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة الفعلية في التمثيل الداخلي. |

