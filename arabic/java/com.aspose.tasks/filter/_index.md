---
title: "Filter"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مرشحًا في Project."
type: docs
weight: 91
url: /ar/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

يمثل مرشحًا في Project.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Filter()](#Filter--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | يقارن هذه الحالة بالنسخة المحددة من فئة [Filter](../../com.aspose.tasks/filter) ويعيد إشارة إلى ترتيبها النسبي. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد. |
| [equals(Object obj)](#equals-java.lang.Object-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد. |
| [getCriteria()](#getCriteria--) | يحصل على المعايير التي يجب أن تفي بها المهام أو الموارد لتظهر في عرض MSP. |
| [getFilterType()](#getFilterType--) | يحصل على نوع الفلتر. |
| [getIndex()](#getIndex--) | يحصل على فهرس كائن [Filter](../../com.aspose.tasks/filter) في كائن Filters الحاوي. |
| [getName()](#getName--) | يحصل على اسم كائن Filter. |
| [getShowInMenu()](#getShowInMenu--) | يحصل على قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في القائمة المنسدلة Filter على علامة تبويب View في Ribbon. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | يحصل على قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر. |
| [getUid()](#getUid--) | يحصل على المعرف الفريد للفلتر. |
| [hashCode()](#hashCode--) | يعيد قيمة رمز التجزئة للفلتر. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من كائن محدد. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من أو مساوية لكائن محدد. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من كائن محدد. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من أو مساوية لكائن محدد. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | يضبط المعايير التي يجب أن تفي بها المهام أو الموارد لتظهر في عرض MSP. |
| [setFilterType(int value)](#setFilterType-int-) | نوع الفلتر. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم كائن Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | يضبط قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في القائمة المنسدلة Filter على علامة تبويب View في Ribbon. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | يضبط قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


يقارن هذه الحالة بالنسخة المحددة من فئة [Filter](../../com.aspose.tasks/filter) ويعيد إشارة إلى ترتيبها النسبي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | الكائن المحدد من فئة [Filter](../../com.aspose.tasks/filter) للمقارنة مع هذا الكائن. |

**Returns:**
int - إشارة إلى ترتيبهم النسبي.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | الكائن AssignmentBaseline المحدد للمقارنة مع هذه الحالة. |

**Returns:**
boolean - يعيد true إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد؛ وإلا false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن AssignmentBaseline المحدد للمقارنة مع هذه الحالة. |

**Returns:**
boolean - يعيد true إذا كانت هذه الحالة مساوية لكائن AssignmentBaseline المحدد؛ وإلا false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


يحصل على المعايير التي يجب أن تفي بها المهام أو الموارد لتظهر في عرض MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


يحصل على نوع الفلتر.

**Returns:**
int - نوع الفلتر.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


يحصل على فهرس كائن [Filter](../../com.aspose.tasks/filter) في كائن Filters الحاوي.

**Returns:**
int - فهرس كائن [Filter](../../com.aspose.tasks/filter) في كائن Filters الحاوي.
### getName() {#getName--}
```
public final String getName()
```


يحصل على اسم كائن Filter.

**Returns:**
java.lang.String - اسم كائن Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


يحصل على قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في القائمة المنسدلة Filter على علامة تبويب View في Ribbon.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في قائمة الفلتر المنسدلة في علامة تبويب العرض على الشريط.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


يحصل على قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر.

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر.
### getUid() {#getUid--}
```
public final int getUid()
```


يحصل على المعرف الفريد للفلتر.

**Returns:**
عدد صحيح - المعرف الفريد للفلتر.
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعيد قيمة رمز التجزئة للفلتر.

**Returns:**
عدد صحيح - يُعيد قيمة رمز التجزئة لهذا الكائن.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن محدد
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من كائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة أكبر من كائن محدد
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أكبر من أو مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة أكبر من أو مساوية لكائن محدد
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة غير مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة غير مساوية لكائن محدد
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من كائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة أصغر من كائن محدد
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


يعيد قيمة تشير إلى ما إذا كانت هذه الحالة أصغر من أو مساوية لكائن محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | الفلتر الأول. |
| b | [Filter](../../com.aspose.tasks/filter) | الفلتر الثاني. |

**Returns:**
منطقي - قيمة تشير إلى ما إذا كانت هذه المثيلة أصغر من أو مساوية لكائن محدد
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


يضبط المعايير التي يجب أن تفي بها المهام أو الموارد لتظهر في عرض MSP.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | المعايير التي يجب أن تفي بها المهام أو الموارد لتُعرض في عرض MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


نوع الفلتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | نوع الفلتر. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


يضبط اسم كائن Filter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم كائن الفلتر. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في القائمة المنسدلة Filter على علامة تبويب View في Ribbon.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كان المشروع يعرض اسم الفلتر في قائمة الفلتر المنسدلة في علامة تبويب العرض على الشريط. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | منطقي | قيمة تشير إلى ما إذا كانت صفوف الملخص المرتبطة تُعرض للفلتر. |

