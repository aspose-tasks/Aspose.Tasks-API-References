---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API 参考"
description: "Projects 视图类"
type: docs
weight: 111
url: /zh/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

项目视图类
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | 初始化一个新的 GanttChartColumn 类实例。 |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | 初始化一个新的 GanttChartColumn 类实例。 |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | 初始化一个新的 GanttChartColumn 类实例。 |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | 初始化一个新的 GanttChartColumn 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | 将当前任务转换为列文本。 |
| [getField()](#getField--) | 返回列字段。 |
| [setField(int value)](#setField-int-) | 设置列字段。 |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


初始化一个新的 GanttChartColumn 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列的名称。 |
| width | int | 列的宽度（像素）。 |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | 任务数据到列文本的转换器。 |
| 字段 | int | 列字段。 |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


初始化一个新的 GanttChartColumn 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列的名称。 |
| width | int | 列的宽度（像素）。 |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | 任务数据到列文本的转换器。 |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


初始化一个新的 GanttChartColumn 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| width | int | 列宽（像素）。 |
| 字段 | int | 列字段。 |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


初始化一个新的 GanttChartColumn 类实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 列名。 |
| width | int | 列宽（像素）。 |
| 字段 | int | 列字段。 |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


将当前任务转换为列文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 当前任务。 |

**Returns:**
java.lang.String - 列文本。
### getField() {#getField--}
```
public int getField()
```


返回列字段。`Field`。

**Returns:**
int - 列字段值。
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


设置列字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 列字段值。 |

