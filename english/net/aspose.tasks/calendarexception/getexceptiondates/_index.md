---
title: CalendarException.GetExceptionDates
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException method. Returns dates on which the calendar exception is applicable
type: docs
weight: 190
url: /net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Returns dates on which the calendar exception is applicable.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Return Value

Returns a collection of exception dates the calendar exception is applicable for.

## Examples

Shows how to get dates for which a specific calendar exception is effective.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### See Also

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


