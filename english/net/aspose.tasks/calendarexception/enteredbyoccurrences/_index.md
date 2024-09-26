---
title: CalendarException.EnteredByOccurrences
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets or sets a value indicating whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date
type: docs
weight: 40
url: /net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Gets or sets a value indicating whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date.

```csharp
public bool EnteredByOccurrences { get; set; }
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


