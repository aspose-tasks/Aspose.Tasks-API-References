---
title: Class RecurringTaskInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RecurringTaskInfo class. Represents the details of a recurring task in a project
type: docs
weight: 1700
url: /net/aspose.tasks/recurringtaskinfo/
---
## RecurringTaskInfo class

Represents the details of a recurring task in a project.

```csharp
public class RecurringTaskInfo
```

## Properties

| Name | Description |
| --- | --- |
| [DailyRepetitions](../../aspose.tasks/recurringtaskinfo/dailyrepetitions/) { get; set; } | Gets or sets a number of repetitions for the daily recurrence pattern. |
| [DailyUseWorkdays](../../aspose.tasks/recurringtaskinfo/dailyuseworkdays/) { get; set; } | Gets or sets a value indicating whether to use workdays for the daily recurrence pattern. |
| [Duration](../../aspose.tasks/recurringtaskinfo/duration/) { get; set; } | Gets or sets the duration for one occurrence of the recurring task. the instance of [`Duration`](./duration/) class. |
| [EndDate](../../aspose.tasks/recurringtaskinfo/enddate/) { get; set; } | Gets or sets the date for the occurrences to end. |
| [MonthlyDay](../../aspose.tasks/recurringtaskinfo/monthlyday/) { get; set; } | Gets or sets a number of day of the monthly recurrence pattern. |
| [MonthlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyordinalday/) { get; set; } | Gets or sets a day of the monthly recurrence pattern when using ordinal day. Can be one of the values of DayOfWeek enumeration. |
| [MonthlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/monthlyordinalnumber/) { get; set; } | Gets or sets an ordinal number of the monthly recurrence pattern. Can be one of the values of [`OrdinalNumber`](../ordinalnumber/) enumeration. |
| [MonthlyOrdinalRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyordinalrepetitions/) { get; set; } | Gets or sets a number of repetitions for the monthly recurrence pattern when using ordinal day. |
| [MonthlyRepetitions](../../aspose.tasks/recurringtaskinfo/monthlyrepetitions/) { get; set; } | Gets or sets a number of repetitions for the monthly recurrence pattern. |
| [MonthlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/monthlyuseordinalday/) { get; set; } | Gets or sets a value indicating whether to use ordinal day for the monthly recurrence pattern. |
| [Occurrences](../../aspose.tasks/recurringtaskinfo/occurrences/) { get; set; } | Gets or sets a number of occurrences of the recurring task. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskinfo/recurrencepattern/) { get; set; } | Gets or sets a recurrence pattern of the recurring task. Can be one of the values of [`RecurrencePattern`](./recurrencepattern/) enumeration. |
| [StartDate](../../aspose.tasks/recurringtaskinfo/startdate/) { get; set; } | Gets or sets the date for the occurrences to begin. |
| [Task](../../aspose.tasks/recurringtaskinfo/task/) { get; } | Gets the parent task of this instance of `RecurringTaskInfo` class. |
| [UseEndDate](../../aspose.tasks/recurringtaskinfo/useenddate/) { get; set; } | Gets or sets a value indicating whether to use the end date or a number of occurrences for the recurring task. |
| [WeeklyDays](../../aspose.tasks/recurringtaskinfo/weeklydays/) { get; set; } | Gets or sets a collection of days used in the weekly recurrence pattern. |
| [WeeklyRepetitions](../../aspose.tasks/recurringtaskinfo/weeklyrepetitions/) { get; set; } | Gets or sets a number of repetitions for the weekly recurrence pattern. |
| [YearlyDate](../../aspose.tasks/recurringtaskinfo/yearlydate/) { get; set; } | Gets or sets a date for the yearly recurrence pattern. |
| [YearlyOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyordinalday/) { get; set; } | Gets or sets a weekday of the yearly recurrence pattern when using ordinal day. Can be one of the values of DayOfWeek enumeration. |
| [YearlyOrdinalMonth](../../aspose.tasks/recurringtaskinfo/yearlyordinalmonth/) { get; set; } | Gets or sets a month of the yearly recurrence pattern when using ordinal day. Can be one of the values of [`Month`](../month/) enumeration. |
| [YearlyOrdinalNumber](../../aspose.tasks/recurringtaskinfo/yearlyordinalnumber/) { get; set; } | Gets or sets an ordinal number of the yearly recurrence pattern. Can be one of the values of [`OrdinalNumber`](../ordinalnumber/) enumeration. |
| [YearlyUseOrdinalDay](../../aspose.tasks/recurringtaskinfo/yearlyuseordinalday/) { get; set; } | Gets or sets a value indicating whether to use ordinal day for the yearly recurrence pattern. |

## Examples

Shows how to read with recurring info of tasks.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

// read recurring information of tasks
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    var info = task.RecurringInfo;
    if (info == null)
    {
        continue;
    }

    Console.WriteLine("Start Date: " + info.StartDate);
    Console.WriteLine("Duration: " + info.Duration);
    Console.WriteLine("End Date: " + info.EndDate);
    Console.WriteLine("Daily Repetitions: " + info.DailyRepetitions);
    Console.WriteLine("Daily Use Workdays: " + info.DailyUseWorkdays);
    Console.WriteLine("Monthly Day: " + info.MonthlyDay);
    Console.WriteLine("Monthly Ordinal Day: " + info.MonthlyOrdinalDay);
    Console.WriteLine("Monthly Ordinal Number: " + info.MonthlyOrdinalNumber);
    Console.WriteLine("Monthly Ordinal Repetitions: " + info.MonthlyOrdinalRepetitions);
    Console.WriteLine("Monthly Repetitions: " + info.MonthlyRepetitions);
    Console.WriteLine("Monthly Use Ordinal Day: " + info.MonthlyUseOrdinalDay);
    Console.WriteLine("Occurrences: " + info.Occurrences);
    Console.WriteLine("Recurrence Pattern: " + info.RecurrencePattern);
    Console.WriteLine("Parent Task: " + info.Task.Get(Tsk.Name));
    Console.WriteLine("Use End Date: " + info.UseEndDate);
    Console.WriteLine("Weekly Days: " + info.WeeklyDays);
    Console.WriteLine("Weekly Repetitions: " + info.WeeklyRepetitions);
    Console.WriteLine("Yearly Date: " + info.YearlyDate);
    Console.WriteLine("Yearly Ordinal Day: " + info.YearlyOrdinalDay);
    Console.WriteLine("Yearly Ordinal Month: " + info.YearlyOrdinalMonth);
    Console.WriteLine("Yearly Ordinal Number: " + info.YearlyOrdinalNumber);
    Console.WriteLine("Yearly Use Ordinal Day: " + info.YearlyUseOrdinalDay);
    Console.WriteLine();
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


