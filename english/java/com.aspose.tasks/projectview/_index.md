---
title: ProjectView
second_title: Aspose.Tasks for Java API Reference
description: Projects view class
type: docs
weight: 227
url: /java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Project's view class
## Constructors

| Constructor | Description |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Initializes a new instance of the [ProjectView](../../com.aspose.tasks/projectview) class. |
## Methods

| Method | Description |
| --- | --- |
| [getColumns()](#getColumns--) | Gets the project view columns. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Includes Uid, task name, resource name, work and duration assignment columns. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Includes id, indicators, name, duration, start and finish task columns. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Includes Uid, resource name, type, material label, initials, group, max units, standard rate, overtime rate, cost per use, accrue at, base calendar and code resource columns. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Includes Uid, name, start, finish and work resource columns. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Includes id, indicators, name, duration, start, finish, predecessors and resource names task columns. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Initializes a new instance of the [ProjectView](../../com.aspose.tasks/projectview) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columns | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | A list of the view columns. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Gets the project view columns.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - the project view columns.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Includes Uid, task name, resource name, work and duration assignment columns.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Includes id, indicators, name, duration, start and finish task columns.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Includes Uid, resource name, type, material label, initials, group, max units, standard rate, overtime rate, cost per use, accrue at, base calendar and code resource columns.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Includes Uid, name, start, finish and work resource columns.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Includes id, indicators, name, duration, start, finish, predecessors and resource names task columns.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
