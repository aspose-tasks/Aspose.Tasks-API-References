---
title: UsageView.MiddleTimescaleTier
second_title: Aspose.Tasks for .NET API Reference
description: UsageView property. Gets or sets settings of views middle timescale tier. TimescaleTier
type: docs
weight: 50
url: /net/aspose.tasks/usageview/middletimescaletier/
---
## UsageView.MiddleTimescaleTier property

Gets or sets settings of view's middle timescale tier. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier MiddleTimescaleTier { get; set; }
```

## Examples

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

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


