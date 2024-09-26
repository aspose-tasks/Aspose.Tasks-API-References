---
title: ProjectView.GetDefaultGanttChartView
second_title: Aspose.Tasks for .NET API Reference
description: ProjectView method. Includes id indicators name duration start and finish task columns
type: docs
weight: 30
url: /net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Includes id, indicators, name, duration, start and finish task columns.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Return Value

a view which contains a list of [`GanttChartColumn`](../../ganttchartcolumn/).

## Examples

Shows how to save a project with Gantt chart view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### See Also

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


