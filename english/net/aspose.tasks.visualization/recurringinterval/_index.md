---
title: Class RecurringInterval
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.RecurringInterval class. Represents recurring intervals used in progress lines of a Gantt Chart view
type: docs
weight: 3290
url: /net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Represents recurring intervals used in progress lines of a Gantt Chart view.

```csharp
public class RecurringInterval
```

## Constructors

| Name | Description |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Gets or sets the daily day number. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Gets or sets a value indicating whether a day is workday for daily progress lines. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Gets or sets the recurring interval. Can be any value of [`Interval`](./interval/) type. |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Gets or sets a value indicating whether to show monthly progress lines by day. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Gets or sets the day number of monthly progress lines. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Gets or sets the month number of monthly progress lines. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Gets or sets a value indicating whether to show progress lines by first or last predefined day. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Gets or sets the first or the last day type of monthly progress lines. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Gets or sets the month number of progress lines, which are shown by first or last predefined day. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Gets a list of days for weekly progress lines. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Gets or sets the week number for weekly progress lines. |

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


