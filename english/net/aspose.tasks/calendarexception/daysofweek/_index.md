---
title: CalendarException.DaysOfWeek
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets the DayTypeCollection for this object. The days of the week on which the exception is valid
type: docs
weight: 20
url: /net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Gets the DayTypeCollection for this object. The days of the week on which the exception is valid.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Examples

Shows how to define calendar exception by week day.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// create a calendar
var calendar = project.Calendars.Add("Calendar1");

// create calendar exception for every friday
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// check that friday is exceptional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// add the exception to the calendar
calendar.Exceptions.Add(exception);
```

### See Also

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


