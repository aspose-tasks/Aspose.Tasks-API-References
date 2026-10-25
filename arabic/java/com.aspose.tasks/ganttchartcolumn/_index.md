---
title: "GanttChartColumn"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة عرض المشاريع"
type: docs
weight: 111
url: /ar/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

فئة عرض المشروع
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | ينشئ مثلاً جديداً من فئة GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | ينشئ مثلاً جديداً من فئة GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | ينشئ مثلاً جديداً من فئة GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | ينشئ مثلاً جديداً من فئة GanttChartColumn. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | يحوّل المهمة الحالية إلى نص العمود. |
| [getField()](#getField--) | يعيد حقل العمود. |
| [setField(int value)](#setField-int-) | يضبط حقل العمود. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


ينشئ مثلاً جديداً من فئة GanttChartColumn.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | محول بيانات المهمة إلى نص العمود. |
| حقل | int | حقل العمود. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


ينشئ مثلاً جديداً من فئة GanttChartColumn.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | محول بيانات المهمة إلى نص العمود. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


ينشئ مثلاً جديداً من فئة GanttChartColumn.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| width | int | عرض العمود بالبكسل. |
| حقل | int | حقل العمود. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


ينشئ مثلاً جديداً من فئة GanttChartColumn.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| حقل | int | حقل العمود. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


يحوّل المهمة الحالية إلى نص العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | المهمة الحالية. |

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

