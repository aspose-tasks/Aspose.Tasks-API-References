---
title: SaveOptions.TimescaleFitBehavior
second_title: Aspose.Tasks for .NET API Reference
description: SaveOptions property. Gets or sets a behavior which define how to align right end of the timescale with the page end
type: docs
weight: 200
url: /net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Gets or sets a behavior which define how to align right end of the timescale with the page end.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Examples

Shows how to use TimescaleFitBehavior make Gantt chart's timescale fit to the end of the last page.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### See Also

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


