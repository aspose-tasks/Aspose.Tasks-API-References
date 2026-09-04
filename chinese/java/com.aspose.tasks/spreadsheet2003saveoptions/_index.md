---
title: "Spreadsheet2003SaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "允许在将项目页面渲染为 Spreadsheet2003 时指定其他选项。"
type: docs
weight: 280
url: /zh/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

允许在将项目页面渲染为 Spreadsheet2003 时指定其他选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | 初始化 [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | 获取要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [getResourceView()](#getResourceView--) | 获取要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [getView()](#getView--) | 获取要保存的视图列的列表 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | 设置要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | 设置要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 设置要保存的视图列的列表 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


初始化 [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions) 类的新实例。

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


获取要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


获取要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


获取要保存的视图列的列表 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。如果未设置，则保存默认列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


设置要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要呈现的分配视图列的列表 ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn))。 |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


设置要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要呈现的资源视图列的列表 ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn))。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


设置要保存的视图列的列表 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。如果未设置，则保存默认列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要保存的视图列的列表 ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn))。 |

