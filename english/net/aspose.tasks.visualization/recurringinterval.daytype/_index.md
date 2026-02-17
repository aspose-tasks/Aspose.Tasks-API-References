---
title: Enum RecurringInterval.DayType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.RecurringIntervalDayType enum. Represents a day type used in progress lines
type: docs
weight: 3300
url: /net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

Represents a day type used in progress lines.

```csharp
public enum DayType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Sunday | `1` | Indicates Sunday. |
| Monday | `2` | Indicates Monday. |
| Tuesday | `3` | Indicates Tuesday. |
| Wednesday | `4` | Indicates Wednesday. |
| Thursday | `5` | Indicates Thursday. |
| Friday | `6` | Indicates Friday. |
| Saturday | `7` | Indicates Saturday. |
| Day | `8` | Indicates Day. |
| Workday | `9` | Indicates Working day. |
| NonworkingDay | `10` | Indicates Nonworking day. |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


