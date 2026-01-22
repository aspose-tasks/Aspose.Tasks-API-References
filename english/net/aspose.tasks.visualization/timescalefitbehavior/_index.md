---
title: Enum TimescaleFitBehavior
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TimescaleFitBehavior enum. Represents a behavior used to align timescale area with page width
type: docs
weight: 3410
url: /net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Represents a behavior used to align timescale area with page width.

```csharp
public enum TimescaleFitBehavior
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| DefinedInView | `0` | Calendar section is rendered according to View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage property of the rendered View. |
| NoScaleToEndDate | `1` | Calendar section is rendered exactly to EndDate, even there is an empty space on a page. |
| NoScaleToEndOfPage | `2` | Calendar section is rendered to the end (right side) of the last page. Thus last rendered date may exceed EndDate. |
| ScaleToEndOfPage | `3` | Rendering engine will try to align dates so that EndDate is aligned with the end (right side) of the last page. Corresponds to MS Project's "Page Setup \ View \ Fit timescale to end of page" option enabled. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


