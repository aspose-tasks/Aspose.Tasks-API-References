---
title: Enum GanttBarSize
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GanttBarSize enum. Specifies the height of a bar in points
type: docs
weight: 700
url: /net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Specifies the height of a bar in points.

```csharp
public enum GanttBarSize
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| BarSize6 | `0` | Bar size 6 points. |
| BarSize8 | `1` | Bar size 8 points. |
| BarSize10 | `2` | Bar size 10 points. |
| BarSize12 | `3` | Bar size 12 points. |
| BarSize14 | `4` | Bar size 14 points. |
| BarSize18 | `5` | Bar size 18 points. |
| BarSize24 | `6` | Bar size 24 points. |

## Examples

Shows how to set some useful properties of Gantt chart view.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// set a value indicating whether the bars round to the nearest day
view.BarRounding = false;
// set the height, in points, of the Gantt bars in the Gantt Chart
view.BarSize = GanttBarSize.BarSize24;
// set a value indicating whether rollup bars will be hidden when expanding summary task
view.HideRollupBarsWhenSummaryExpanded = true;
// set non-working time color
view.NonWorkingTimeColor = Color.Azure;
// set a value indicating whether bars on the Gantt Chart must be rolled up
view.RollUpGanttBars = true;
// set a value indicating whether task splits on the Gantt Chart must be shown
view.ShowBarSplits = true;
// set a value indicating whether drawings on the Gantt Chart must be shown
view.ShowDrawings = true;
// set a percentage to reduce or enlarge the spacing between units on the timescale tier
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


