---
title: CalendarException.Occurrences
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets or sets the number of occurrences for which the calendar exception is valid
type: docs
weight: 110
url: /net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Gets or sets the number of occurrences for which the calendar exception is valid.

```csharp
public int Occurrences { get; set; }
```

## Examples

Shows how to define a calendar exception by occurrences.

```csharp
var project = new Project();

// Define a calendar
var calendar = project.Calendars.Add("Calendar1");

// Define exception and specify occurrences
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Add exception to calendar
calendar.Exceptions.Add(exception);
```

### See Also

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


