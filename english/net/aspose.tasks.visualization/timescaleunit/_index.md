---
title: Enum TimescaleUnit
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TimescaleUnit enum. Specifies the unit of time for any tier of a timescale in a Gantt chart or other time phased view
type: docs
weight: 3380
url: /net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

Specifies the unit of time for any tier of a timescale in a Gantt chart or other time phased view.

```csharp
public enum TimescaleUnit
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `-1` | Indicates None. The timescale tier is hidden. |
| Minutes | `0` | Indicates Minutes timescale unit. |
| Hours | `1` | Indicates Hours timescale unit. |
| Days | `2` | Indicates Days timescale unit. |
| Weeks | `3` | Indicates Weeks timescale unit. |
| ThirdsOfMonths | `4` | Indicates Thirds of months timescale unit. |
| Months | `5` | Indicates Months timescale unit. |
| Quarters | `6` | Indicates Quarters of years timescale unit. |
| HalfYears | `7` | Indicates Half years timescale unit. |
| Years | `8` | Indicates Years timescale unit. |

## Examples

Shows how to customize timescale tier labels.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Add task links
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// tune timescale tiers

// tune the top tier
// set the top timescale tier of the Gantt Chart view.
view.MiddleTimescaleTier = new TimescaleTier();
// set timescale unit <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> for the timescale tier.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// set the time unit interval in which to show labels for the tier.
view.MiddleTimescaleTier.Count = 1;
// set date label <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> for the timescale tier.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// set how to align labels within each time period of the tier (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// set a value indicating whether whether to show tick marks that separate time periods in the tier.
view.MiddleTimescaleTier.ShowTicks = true;
// set a value indicating whether to base the tier labels on the fiscal year.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// added for better visualization
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// customize middle tier dates
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Use 'Timescale.DefinedInView' option to render timescales using timescale settings defined in view (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier). 
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


