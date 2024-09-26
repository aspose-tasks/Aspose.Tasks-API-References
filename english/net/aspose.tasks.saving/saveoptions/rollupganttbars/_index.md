---
title: SaveOptions.RollUpGanttBars
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them
type: docs
weight: 160
url: /net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Gets or sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Remarks

Is only applicable when Gantt chart view is rendered.

## Examples

Shows how to set a value indicating that subtasks on the summary task bar must be rolled up.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // OR
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### See Also

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


