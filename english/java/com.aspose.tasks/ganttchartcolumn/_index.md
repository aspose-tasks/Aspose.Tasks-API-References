---
title: GanttChartColumn
second_title: Aspose.Tasks for Java API Reference
description: Projects view class
type: docs
weight: 111
url: /java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Project's view class
## Constructors

| Constructor | Description |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Initializes a new instance of the GanttChartColumn class. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Initializes a new instance of the GanttChartColumn class. |
## Methods

| Method | Description |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Converts current task to the column text. |
| [getField()](#getField--) | Returns column field. |
| [setField(int value)](#setField-int-) | Sets column field. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Initializes a new instance of the GanttChartColumn class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column's name. |
| width | int | Column's width in pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Task data to column text converter. |
| field | int | Column field. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Initializes a new instance of the GanttChartColumn class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column's name. |
| width | int | Column's width in pixels. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Task data to column text converter. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Initializes a new instance of the GanttChartColumn class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | int | Column width in pixels. |
| field | int | Column field. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Initializes a new instance of the GanttChartColumn class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Column name. |
| width | int | Column width in pixels. |
| field | int | Column field. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Converts current task to the column text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Current task. |

**Returns:**
java.lang.String - The column text.
### getField() {#getField--}
```
public int getField()
```


Returns column field. `Field`.

**Returns:**
int - column field value.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Sets column field.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | column field value. |

