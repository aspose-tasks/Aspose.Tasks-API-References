---
title: "ExtendedAttribute"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل السمات الموسعة."
type: docs
weight: 81
url: /ar/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

يمثل السمات الموسعة.

--------------------

حاليًا يتم دعم جميع أنواع السمات الموسعة المقروءة من MSP Xml 2003/2007 و mpp 2003. بالنسبة إلى MSP mpp 2007 يتم دعم قراءة جميع السمات الموسعة باستثناء الفترات الزمنية والعلامات.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | يحصل على تعريف السمة. |
| [getDateValue()](#getDateValue--) | يحصل على قيمة للسمات ذات أنواع التاريخ (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | يحصل على القيمة للسمات من النوع 'Duration'. |
| [getFieldId()](#getFieldId--) | يحصل على معرف الحقل. |
| [getFlagValue()](#getFlagValue--) | يحصل على قيمة تشير إلى ما إذا كان العلم مفعلاً للسمات من النوع 'Flag'. |
| [getNumericValue()](#getNumericValue--) | يحصل على قيمة للسمات ذات الأنواع الرقمية (Cost, Number). |
| [getTextValue()](#getTextValue--) | يحصل على قيمة للسمات من النوع 'Text'. |
| [getValueGuid()](#getValueGuid--) | يحصل على الـ guid لقيمة البحث. |
| [getValueReadOnly()](#getValueReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت قيمة هذا الكائن [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) للقراءة فقط. |
| [isErrorValue()](#isErrorValue--) | يحصل على ما إذا كان حساب قيمة السمة الموسعة قد نتج عنه خطأ. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | يضبط قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | يضبط قيمة للسمات من النوع 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | يضبط قيمة تشير إلى ما إذا كان العلم مفعلاً للسمات من النوع 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | يضبط قيمة للسمات ذات الأنواع الرقمية (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | يضبط قيمة للسمات من النوع 'Text'. |
| [toString()](#toString--) | يرجع تمثيل نصي قصير لسمة موسعة. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


يحصل على تعريف السمة.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


يحصل على قيمة للسمات ذات أنواع التاريخ (Date, Start, Finish).

**Returns:**
java.util.Date - قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


يحصل على القيمة للسمات من النوع 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


يحصل على معرف الحقل.

**Returns:**
java.lang.String - معرف الحقل.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


يحصل على قيمة تشير إلى ما إذا كان العلم مفعلاً للسمات من النوع 'Flag'.

**Returns:**
boolean - قيمة تشير إلى ما إذا كان العلم مفعلاً للسمات من النوع 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


يحصل على قيمة للسمات ذات الأنواع الرقمية (Cost, Number).

**Returns:**
java.math.BigDecimal - قيمة للسمات ذات الأنواع الرقمية (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


يحصل على قيمة للسمات من النوع 'Text'.

**Returns:**
java.lang.String - قيمة للسمات من النوع 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


يحصل على الـ guid لقيمة البحث.

--------------------

يجب عدم ضبطه مباشرةً، بل استخدم ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) لإنشاء سمة موسعة بقيمة بحث.

**Returns:**
java.lang.String - الـ guid لقيمة البحث.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت قيمة هذا الكائن [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) للقراءة فقط.

Value: يرجع true إذا تم تعريف صيغة أو تجميع في [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) لهذا الكائن.

**Returns:**
boolean - قيمة تشير إلى ما إذا كانت قيمة هذا الكائن [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) للقراءة فقط.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


يحصل على ما إذا كان حساب قيمة السمة الموسعة قد نتج عنه خطأ.

**Returns:**
boolean - ما إذا كان حساب قيمة السمة الموسعة قد نتج عنه خطأ.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


يضبط قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة للسمات ذات الأنواع التاريخية (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


يضبط قيمة للسمات من النوع 'Duration'.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | قيمة للسمات من نوع 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان العلم مفعلاً للسمات من النوع 'Flag'.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا تم تعيين علامة لسمات من نوع 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


يضبط قيمة للسمات ذات الأنواع الرقمية (Cost, Number).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.math.BigDecimal | قيمة للسمات ذات الأنواع الرقمية (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


يضبط قيمة للسمات من النوع 'Text'.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة للسمات من نوع 'Text'. |

### toString() {#toString--}
```
public String toString()
```


يرجع تمثيل نصي قصير لسمة موسعة.

**Returns:**
java.lang.String - تمثيل السلسلة للخاصية الموسعة.
