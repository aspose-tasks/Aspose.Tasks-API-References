---
title: CalendarException.GetWorkingTime
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException method. Returns the working time for a calendar exception
type: docs
weight: 200
url: /net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Returns the working time for a calendar exception.

```csharp
public TimeSpan GetWorkingTime()
```

### Return Value

Returns working time for this calendar exception.

## Examples

Shows how to get a working time of a calendar exception.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### See Also

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


