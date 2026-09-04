---
title: "GraphicalIndicatorCriteria"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل معيار مؤشر رسومي واحد مرتبط بصفة موسعة."
type: docs
weight: 115
url: /ar/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

يمثل معيار مؤشر رسومي واحد مرتبط بصفة موسعة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | يُنشئ مثيلاً جديدًا من النوع [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | يُنشئ مثيلاً جديدًا من النوع [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | يحصل على فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير. |
| [getRowType()](#getRowType--) | يحصل على قيمة تعداد [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) الذي يحدد الصفوف التي يُطبق عليها المؤشر. |
| [getTest()](#getTest--) | يحصل على نوع المقارنة التي تُجرى بين قيمة السمة الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي. |
| [getValue1()](#getValue1--) | يحصل على القيمة المستخدمة لاختبار قيمة السمة الموسعة. |
| [getValue2()](#getValue2--) | يحصل على القيمة الثانية المستخدمة لاختبار قيمة السمة الموسعة في حالة أنواع المقارنة 'IsWithin' و 'IsNotWithin'. |
| [toString()](#toString--) | يرجع تمثيلًا نصيًا لمثيل الفئة [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


يُنشئ مثيلاً جديدًا من النوع [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowType | int | قيمة تعداد [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) الذي يحدد الصفوف التي يُطبق عليها المؤشر. |
| test | int | قيمة [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) التي تشير إلى نوع المقارنة التي يجريها المعيار. |
| imageIndex | int | فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | القيم المستخدمة في فحص الشرط. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | القيمة الثانية (نهاية الفاصل) المستخدمة في فحص الشرط في حالة شروط 'IsWithin' و 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


يُنشئ مثيلاً جديدًا من النوع [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowType | int | قيمة تعداد [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) الذي يحدد الصفوف التي يُطبق عليها المؤشر. |
| test | int | قيمة [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) التي تشير إلى نوع المقارنة التي يجريها المعيار. |
| imageIndex | int | فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | القيمة المستخدمة في فحص الشرط. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


يحصل على فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير.

**Returns:**
int - فهرس الصورة التي سيتم عرضها عندما يفي الحقل بالمعايير.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


يحصل على قيمة تعداد [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) الذي يحدد الصفوف التي يُطبق عليها المؤشر.

**Returns:**
int - قيمة تعداد [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) الذي يحدد الصفوف التي يُطبق عليها المؤشر.
### getTest() {#getTest--}
```
public final int getTest()
```


يحصل على نوع المقارنة التي تُجرى بين قيمة السمة الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - نوع المقارنة التي تُجرى بين قيمة السمة الموسعة والقيم التي تعمل كمعيار لتطبيق المؤشر الرسومي.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


يحصل على القيمة المستخدمة لاختبار قيمة السمة الموسعة.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


يحصل على القيمة الثانية المستخدمة لاختبار قيمة السمة الموسعة في حالة أنواع المقارنة 'IsWithin' و 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


يرجع تمثيلًا نصيًا لمثيل الفئة [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - تمثيل نصي لهذا الكائن.
