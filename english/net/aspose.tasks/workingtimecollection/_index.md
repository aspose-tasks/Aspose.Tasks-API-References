---
title: Class WorkingTimeCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WorkingTimeCollection class. Represents a collection of WorkingTimeCollection objects
type: docs
weight: 3590
url: /net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Represents a collection of `WorkingTimeCollection` objects.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Gets the number of objects contained in this `WorkingTimeCollection` object. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Returns the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Adds a new WorkingTime instance to this collection. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Removes all [`WorkingTime`](../workingtime/) items from collection. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Checks if the specified element is in the List. Performs a linear O(n) search. |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | copies a collection content into an Array, starting at a particular index |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Removes [`WorkingTime`](../workingtime/) instance from this collection. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Converts the WorkingTimeCollection object to a list of [`WorkingTime`](../workingtime/) objects. |

## Examples

Shows how to work with working time collection.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// print working times of Saturday
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// print working times of sunday
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // You can further traverse through working times and display these
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### See Also

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


