---
title: ProjectView.GetDefaultTaskSheetView
second_title: Aspose.Tasks for .NET API Reference
description: ProjectView method. Includes id indicators name duration start finish predecessors and resource names task columns
type: docs
weight: 60
url: /net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Includes id, indicators, name, duration, start, finish, predecessors and resource names task columns.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Return Value

a view which contains a list of [`GanttChartColumn`](../../ganttchartcolumn/).

## Examples

Shows how to save a project with task sheet view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### See Also

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


