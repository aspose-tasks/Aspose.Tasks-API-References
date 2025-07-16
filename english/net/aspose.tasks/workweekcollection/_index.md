---
title: Class WorkWeekCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkWeekCollection class. Represents a collection of WorkWeek objects
type: docs
weight: 3570
url: /net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Represents a collection of [`WorkWeek`](../workweek/) objects.

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Gets the number of objects contained in this `WorkWeekCollection` object. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Gets the parent calendar. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Adds WorkWeek instance to this collection object. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Converts the WorkWeekCollection object to a list of [`WorkWeek`](../workweek/) objects. |

## Examples

Shows how to create a custom work week for a calendar.

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


