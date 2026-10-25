---
title: "AssignmentViewColumn"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة عرض المشاريع."
type: docs
weight: 19
url: /ar/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

فئة عرض المشروع.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | يُنشئ مثلاً جديداً لفئة AssignmentViewColumn. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | يحوّل تعيين المورد الحالي إلى نص العمود. |
| [getField()](#getField--) | يعيد حقل العمود. |
| [setField(int value)](#setField-int-) | يضبط حقل العمود. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


يُنشئ مثلاً جديداً لفئة AssignmentViewColumn.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | محوّل بيانات التعيين إلى نص العمود. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


يحوّل تعيين المورد الحالي إلى نص العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | التعيين الحالي. |

**Returns:**
java.lang.String - نص العمود.
### getField() {#getField--}
```
public int getField()
```


يعيد حقل العمود. `Field`.

**Returns:**
int - قيمة حقل العمود.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


يضبط حقل العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة حقل العمود. |

