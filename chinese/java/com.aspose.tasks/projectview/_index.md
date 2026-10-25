---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API 参考"
description: "Projects 视图类"
type: docs
weight: 228
url: /zh/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

项目视图类
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | 初始化 [ProjectView](../../com.aspose.tasks/projectview) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getColumns()](#getColumns--) | 获取项目视图列。 |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | 包括 Uid、任务名称、资源名称、工作和持续时间分配列。 |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | 包括 id、指示器、名称、持续时间、开始和完成任务列。 |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | 包括 Uid、资源名称、类型、材料标签、缩写、组、最大单位、标准费率、加班费率、每次使用成本、累计时间、基础日历和代码资源列。 |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | 包括 Uid、名称、开始、完成和工作资源列。 |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | 包括 id、指示器、名称、持续时间、开始、完成、前置任务和资源名称任务列。 |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


初始化 [ProjectView](../../com.aspose.tasks/projectview) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | 视图列的列表。 |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


获取项目视图列。

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - 项目视图列。
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


包括 Uid、任务名称、资源名称、工作和持续时间分配列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


包括 id、指示器、名称、持续时间、开始和完成任务列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


包括 Uid、资源名称、类型、材料标签、缩写、组、最大单位、标准费率、加班费率、每次使用成本、累计时间、基础日历和代码资源列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


包括 Uid、名称、开始、完成和工作资源列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


包括 id、指示器、名称、持续时间、开始、完成、前置任务和资源名称任务列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
