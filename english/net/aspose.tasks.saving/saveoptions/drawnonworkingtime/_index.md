---
title: SaveOptions.DrawNonWorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a value indicating whether nonworking time should be drawn Default value is TRUE
type: docs
weight: 30
url: /net/aspose.tasks.saving/saveoptions/drawnonworkingtime/
---
## SaveOptions.DrawNonWorkingTime property

Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE).

```csharp
public bool DrawNonWorkingTime { get; set; }
```

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


