---
title: Class ProgressLines
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.ProgressLines class. Represents progress lines in a Gantt Chart view
type: docs
weight: 3270
url: /net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Represents progress lines in a Gantt Chart view.

```csharp
public class ProgressLines
```

## Constructors

| Name | Description |
| --- | --- |
| [ProgressLines](progresslines/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Gets or sets the date to display progress lines from. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Gets or sets a value indicating whether to display progress lines from the beginning of the project start date. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Gets or sets the date format ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Gets or sets a value indicating whether to display progress line at current date. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Gets or sets a value indicating whether to display progress line at recurring intervals. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Gets or sets a value indicating whether to display progress lines at the selected dates. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Gets or sets the font used for progress line label. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Gets or sets a value indicating whether to display progress lines for baseline plan or actual. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Gets or sets the line color for current progress line. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Gets or sets the line pattern of current progress line. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Gets or sets the color of other progress line. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Gets or sets the line pattern for other progress line. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Gets or sets the color of other progress point. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Gets or sets the progress point shape of other progress line. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Gets or sets the color of progress point. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Gets or sets the progress point shape. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Gets or sets the recurring interval. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Gets the list of selected dates to display progress lines for. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Gets or sets a value indicating whether to show date for each progress line. |

## Examples

Shows how to work with progress lines.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// lets define progress line
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// set the date to display progress lines from. Lets set a project's status date.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// set a value indicating whether to display progress lines from the beginning of the project start date
progressLines.BeginAtProjectStart = true;
// set the date format (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// set a value indicating whether to display progress line at current date.
progressLines.DisplayAtCurrentDate = true;
// set a value indicating whether to display progress line at recurring intervals.
progressLines.DisplayAtRecurringIntervals = true;
// set a value indicating whether to display progress lines at the selected dates
progressLines.DisplaySelected = true;
// set a value indicating whether to display progress lines for baseline plan or actual.
progressLines.IsBaselinePlan = false;
// set the font used for progress line label.
progressLines.Font = new FontDescriptor("Arial", 10);
// set the line color for current progress line.
progressLines.LineColor = Color.Aquamarine;
// set the line pattern of current progress line.
progressLines.LinePattern = LinePattern.Dashed;
// set the color of other progress line.
progressLines.OtherLineColor = Color.Azure;
// set the line pattern for other progress line.
progressLines.OtherLinePattern = LinePattern.Dotted;
// set the color of other progress point.
progressLines.OtherProgressPointColor = Color.Red;
// set the progress point shape of other progress line.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// set the color of progress point.
progressLines.ProgressPointColor = Color.Orange;
// set the progress point shape.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// set the recurring interval.
progressLines.RecurringInterval = new RecurringInterval();
// set the recurring interval.
progressLines.RecurringInterval.Interval = Interval.Daily;
// set the daily day number
progressLines.RecurringInterval.DailyDayNumber = 1;
// set a value indicating whether to show date for each progress line.
progressLines.ShowDate = true;

// lets check progress lines
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


