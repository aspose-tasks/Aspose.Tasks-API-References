---
title: CalendarException.WorkingTimes
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets or sets the WorkingTimeCollection object. The collection of working times that defines the time worked on the weekday.  At least one working time must present and there cant be more than five
type: docs
weight: 160
url: /net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Gets or sets the WorkingTimeCollection object. The collection of working times that defines the time worked on the weekday.  At least one working time must present, and there can't be more than five.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


