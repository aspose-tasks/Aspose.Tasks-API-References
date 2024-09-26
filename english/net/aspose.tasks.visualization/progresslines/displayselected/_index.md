---
title: ProgressLines.DisplaySelected
second_title: Aspose.Tasks for .NET API Reference
description: ProgressLines property. Gets or sets a value indicating whether to display progress lines at the selected dates
type: docs
weight: 70
url: /net/aspose.tasks.visualization/progresslines/displayselected/
---
## ProgressLines.DisplaySelected property

Gets or sets a value indicating whether to display progress lines at the selected dates.

```csharp
public bool DisplaySelected { get; set; }
```

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

* class [ProgressLines](../)
* namespace [Aspose.Tasks.Visualization](../../progresslines/)
* assembly [Aspose.Tasks](../../../)


