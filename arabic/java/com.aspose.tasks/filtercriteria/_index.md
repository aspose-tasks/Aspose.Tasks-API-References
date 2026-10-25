---
title: "FilterCriteria"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يحدد المعايير التي يجب أن تلبيها المهام أو الموارد لتظهر في عرض MSP."
type: docs
weight: 94
url: /ar/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

يحدد المعايير التي يجب أن تلبيها المهام أو الموارد لتظهر في عرض MSP.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | يحصل على قائمة الصفوف الفرعية لـ [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows. |
| [getField()](#getField--) | يحصل على `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغييره. |
| [getOperation()](#getOperation--) | يحصل على المعيار الذي تم إنشاؤه باستخدام FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر. |
| [getTest()](#getTest--) | يحصل على نوع المقارنة الذي يتم إجراؤه بين FieldName و Value والذي يعمل كمعيار اختيار للفلتر. |
| [getValues()](#getValues--) | يحصل على قيم الكائن للمقارنة مع قيمة الحقل المحدد بـ FieldName. |
| [isValueAField()](#isValueAField--) | يحصل على ما إذا كانت القيمة اليمنى لـ FilterCriteria هي إشارة إلى حقل، وليس قيمة ثابتة. |
| [isValueAField(int index)](#isValueAField-int-) | يحصل على ما إذا كانت القيمة في الفهرس الخاص بـ FilterCriteria هي إشارة إلى حقل، وليس قيمة ثابتة. |
| [setField(int value)](#setField-int-) | يضبط `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغييره. |
| [setOperation(int value)](#setOperation-int-) | يضبط المعيار الذي تم إنشاؤه باستخدام FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر. |
| [setTest(int value)](#setTest-int-) | يضبط نوع المقارنة الذي يتم إجراؤه بين FieldName و Value والذي يعمل كمعيار اختيار للفلتر. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | يضبط قيمة الكائن في الفهرس للمقارنة مع قيمة الحقل المحدد بواسطة FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يضبط قيمة الكائن للمقارنة مع قيمة الحقل المحدد بواسطة FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | يضبط الحقل الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | يضبط الحقل في الفهرس الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName. |
| [toString()](#toString--) | يعيد تمثيل السلسلة للنسخة من فئة [FilterCriteria](../../com.aspose.tasks/filtercriteria) class. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


يحصل على قائمة الصفوف الفرعية لـ [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows. إذا كان الفلتر يحتوي على أكثر من صف معيار واحد، فإن تأثير عامل And هو أن المعايير لكلا الصفين يجب أن تتحقق لكي يتم عرض المهمة أو المورد كنتيجة لهذا الفلتر. تأثير عامل Or هو أن المعايير لواحد من الصفين يجب أن تتحقق.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - قائمة الصفوف الفرعية لـ [FilterCriteria](../../com.aspose.tasks/filtercriteria) rows.
### getField() {#getField--}
```
public final int getField()
```


يحصل على `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغييره.

**Returns:**
int - `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغييره.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


يحصل على المعيار الذي تم إنشاؤه باستخدام FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر.

**Returns:**
int - المعيار الذي تم إنشاؤه باستخدام FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر.
### getTest() {#getTest--}
```
public final int getTest()
```


يحصل على نوع المقارنة الذي يتم إجراؤه بين FieldName و Value والذي يعمل كمعيار اختيار للفلتر. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - نوع المقارنة الذي يتم إجراؤه بين FieldName و Value والذي يعمل كمعيار اختيار للفلتر.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


يحصل على قيم الكائن للمقارنة مع قيمة الحقل المحدد بـ FieldName.

**Returns:**
java.lang.Object[] - قيم الكائن للمقارنة مع قيمة الحقل المحدد بـ FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


يحصل على ما إذا كانت القيمة اليمنى لـ FilterCriteria هي إشارة إلى حقل، وليس قيمة ثابتة.

**Returns:**
boolean - ما إذا كانت القيمة اليمنى لـ FilterCriteria هي إشارة إلى حقل، وليس قيمة ثابتة.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


يحصل على ما إذا كانت القيمة في الفهرس الخاص بـ FilterCriteria هي إشارة إلى حقل، وليس قيمة ثابتة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | فهرس القيمة |

**Returns:**
منطقي - ما إذا كانت القيمة اليمنى في الفهرس FilterCriteria إشارة إلى حقل، وليس قيمة ثابتة.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


يضبط `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغييره.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | int | `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) لتغيير. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


يضبط المعيار الذي تم إنشاؤه باستخدام FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | المعيار المحدد بـ FieldName و Test و Value يتعلق بمعايير أخرى في الفلتر. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


يضبط نوع المقارنة بين FieldName و Value الذي يعمل كمعيار اختيار للفلتر. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع المقارنة بين FieldName و Value الذي يعمل كمعيار اختيار للفلتر. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


يضبط قيمة الكائن في الفهرس للمقارنة مع قيمة الحقل المحدد بواسطة FieldName.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | فهرس القيمة. |
| القيمة | java.lang.Object | قيمة كائن ستُستخدم كقيمة يمنى في فهرس معايير الفلتر. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


يضبط قيمة الكائن للمقارنة مع قيمة الحقل المحدد بواسطة FieldName.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object | قيمة كائن ستُستخدم كقيمة يمنى لمعايير الفلتر. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


يضبط الحقل الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | حقل سيُستخدم كقيمة يمنى لمعايير الفلتر. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


يضبط الحقل في الفهرس الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | فهرس القيمة |
| القيمة | int | حقل سيُستخدم كقيمة يمنى في فهرس معايير الفلتر. |

### toString() {#toString--}
```
public String toString()
```


يعيد تمثيل السلسلة للنسخة من فئة [FilterCriteria](../../com.aspose.tasks/filtercriteria) class.

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن.
