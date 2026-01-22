---
title: Class ProjectView
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.ProjectView class. Projects view class
type: docs
weight: 3270
url: /net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Project's view class

```csharp
public class ProjectView
```

## Constructors

| Name | Description |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Initializes a new instance of the `ProjectView` class. |

## Properties

| Name | Description |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Gets the project view columns. |

## Methods

| Name | Description |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Includes Uid, task name, resource name, work and duration assignment columns. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Includes id, indicators, name, duration, start and finish task columns. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Includes Uid, resource name, type, material label, initials, group, max units, standard rate, overtime rate, cost per use, accrue at, base calendar and code resource columns. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Includes Uid, name, start, finish and work resource columns. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Includes id, indicators, name, duration, start, finish, predecessors and resource names task columns. |

## Examples

Shows how to save a project with assignment view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


