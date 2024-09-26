---
title: CalendarException.Delete
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException method. Deletes the Exception instance from parent calendar CalendarExceptionCollection object
type: docs
weight: 180
url: /net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Deletes the Exception instance from parent calendar CalendarExceptionCollection object.

```csharp
public void Delete()
```

## Examples

Shows how to delete a calendar exception.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// remove the exception
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### See Also

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


