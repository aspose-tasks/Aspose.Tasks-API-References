---
title: GanttChartView.BarSize
second_title: Aspose.Tasks for .NET API Reference
description: GanttChartView property. Gets or sets the height in points of the Gantt bars in the Gantt Chart
type: docs
weight: 40
url: /net/aspose.tasks/ganttchartview/barsize/
---
## GanttChartView.BarSize property

Gets or sets the height, in points, of the Gantt bars in the Gantt Chart.

```csharp
public GanttBarSize BarSize { get; set; }
```

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

* enum [GanttBarSize](../../ganttbarsize/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


