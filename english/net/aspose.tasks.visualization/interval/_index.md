---
title: Enum Interval
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.Interval enum. Specifies recurring intervals to display progress lines at
type: docs
weight: 3140
url: /net/aspose.tasks.visualization/interval/
---
## Interval enumeration

Specifies recurring intervals to display progress lines at.

```csharp
public enum Interval
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Daily | `0` | Indicates Daily interval. |
| Weekly | `1` | Indicates Weekly interval. |
| Monthly | `2` | Indicates Monthly interval. |

## Examples

Shows how to work with recurring interval of progress lines.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// lets read progress line
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// lets redefine recurring interval
var newInterval = new RecurringInterval();

// set a value indicating whether to show monthly progress lines by day.
interval.MonthlyDay = true;
// set the day number of monthly progress lines.
interval.MonthlyDayDayNumber = 1;
// set the month number of monthly progress lines.
interval.MonthlyDayMonthNumber = 1;
// set a value indicating whether to show progress lines by first or last predefined day.
interval.MonthlyFirstLast = true;
// set the first or the last day type of monthly progress lines.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// set the month number of progress lines, which are shown by first or last predefined day.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


