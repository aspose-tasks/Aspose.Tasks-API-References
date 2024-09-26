---
title: Class GanttChartView
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GanttChartView class. Represents a GanttChart view
type: docs
weight: 710
url: /net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Represents a GanttChart view.

```csharp
public class GanttChartView : View
```

## Constructors

| Name | Description |
| --- | --- |
| [GanttChartView](ganttchartview/)() | Initializes a new instance of the `GanttChartView` class. |

## Properties

| Name | Description |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Gets a list of auto filters of a Gantt Chart view. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | Gets or sets a value indicating whether the bars round to the nearest day. The default value is True. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Gets or sets the height, in points, of the Gantt bars in the Gantt Chart. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Gets a list of parent (common) bar styles of the Gantt Chart view. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | Gets or sets settings of view's bottom timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Gets a list of custom task-specific bar styles of the Gantt Chart view. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Gets or sets a filter used in a single view. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Gets or sets a list of [`Gridlines`](./gridlines/) of the Gantt Chart view. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Gets or sets a group of the single view. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | Gets or sets a value indicating whether rollup bars will be hidden when expanding summary task. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Gets or sets a value indicating whether Microsoft Project highlights the filter for a single view. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | Gets or sets settings of view's middle timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Gets or sets the name of a View object. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | Gets or sets non-working time color. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Gets an instance of the [`PageInfo`](../view/pageinfo/) class. Represents page setup data which is present in mpp file format. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Gets the parent of the View object. Read-only [`Project`](../project/). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Gets or sets progress lines for the Gantt Chart view. [`ProgressLines`](./progresslines/). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Gets or sets a value indicating whether bars on the Gantt Chart must be rolled up. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Gets the screen type for the single view. Read-only [`ViewScreen`](../viewscreen/). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Gets or sets a value indicating whether task splits on the Gantt Chart must be shown. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Gets or sets a value indicating whether drawings on the Gantt Chart must be shown. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Gets or sets a value indicating whether Microsoft Project shows the single view name in the View or the Other Views drop-down lists in the Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Gets or sets a table of the single view. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Gets a list of table text styles of the Gantt Chart view. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Gets or sets a list of [`TextStyle`](../../aspose.tasks.visualization/textstyle/) of the Gantt Chart view. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | Gets or sets settings of view's top timescale tier. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Gets the type of item in the single view, such as tasks or resources. Read-only [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Gets the unique identifier of a view. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Gets a collection of objects representing placement and appearance of [`OleObject`](../oleobject/) in the view. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compares the current instance with another object of the same type and returns an integer that indicates whether the current instance precedes, follows, or occurs in the same position in the sort order as the other object. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Returns a hash code value for the instance of the [`Resource`](../resource/) class. |

## Examples

Shows how to modify timescale tiers.

```csharp
var project = new Project();

// Init Gantt Chart View
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// set Time Scale count
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// add Gantt Chart View to project
project.Views.Add(view);

// add some test data to project
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Use 'Timescale.DefinedInView' option to render timescales using timescale settings which we have set (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier). 
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### See Also

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


