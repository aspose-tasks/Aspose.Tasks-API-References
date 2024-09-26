---
title: DayTypeCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: DayTypeCollection property. Gets the number of elements contained in this collection
type: docs
weight: 10
url: /net/aspose.tasks/daytypecollection/count/
---
## DayTypeCollection.Count property

Gets the number of elements contained in this collection.

```csharp
public int Count { get; }
```

## Examples

Shows how to use a week day collection to define weekly calendar exception.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // delete a day type from "Exception 2" by day type
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// delete a day type from "Exception 2" by index
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Change exceptions (there is no exceptions in initial project data)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// remove all days of week for "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### See Also

* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


