---
title: Class WorkWeek
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkWeek class. Represent WorkWeek class
type: docs
weight: 3620
url: /net/aspose.tasks/workweek/
---
## WorkWeek class

Represent WorkWeek class

```csharp
public class WorkWeek
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkWeek](workweek/)() | Initializes a new instance of the `WorkWeek` class. |

## Properties

| Name | Description |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | Gets or sets start DateTime of work week |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | Gets or sets Name of work week |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | Gets or sets Finish DateTime of work week |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Gets week days. |

## Examples

Shows how to read work week information from the project.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Display work week name, parent calendar name, from, and to dates
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // This data is all about "Details." button you can set special working times for special WeekDay or even make it nonworking
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // You can further traverse through working times and display these
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


