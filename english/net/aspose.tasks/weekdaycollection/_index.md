---
title: Class WeekDayCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeekDayCollection class. Represents a collection of WeekDay objects
type: docs
weight: 3500
url: /net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Represents a collection of [`WeekDay`](../weekday/) objects.

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Gets the number of objects contained in this `WeekDayCollection` object. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Gets or sets the item value at specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Adds a [`WeekDay`](../weekday/) instance to this object. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Clear the WeekDayCollection object. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Checks if collection contains [`WeekDay`](../weekday/).specified. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Copies collection content to an array at specified index. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Returns index of [`WeekDay`](../weekday/) specified. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Inserts [`WeekDay`](../weekday/) at specified index. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Removes [`WeekDay`](../weekday/) specified, if any. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Removes an item at specified index. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Converts the WeekDayCollection object to a list of [`WeekDay`](../weekday/) objects. |

## Examples

Shows how to work week day collections.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// clear week days
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// remove saturday week day
calendar.WeekDays.RemoveAt(5);

// remove sunday week day
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// copy week days
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### See Also

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


