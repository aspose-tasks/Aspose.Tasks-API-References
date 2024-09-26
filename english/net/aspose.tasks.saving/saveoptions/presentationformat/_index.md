---
title: SaveOptions.PresentationFormat
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets the PresentationFormat in which the document will be saved
type: docs
weight: 140
url: /net/aspose.tasks.saving/saveoptions/presentationformat/
---
## SaveOptions.PresentationFormat property

Gets or sets the `PresentationFormat` in which the document will be saved.

```csharp
public PresentationFormat PresentationFormat { get; set; }
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

Shows how to render task usage view with timescale settings defined in view settings.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Define the SaveOptions and specify that TaskUsageView timescale settings should be used.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### See Also

* enum [PresentationFormat](../../../aspose.tasks.visualization/presentationformat/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


