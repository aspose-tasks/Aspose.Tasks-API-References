---
title: CalendarException.MonthPosition
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets or sets the position of a month item within a month
type: docs
weight: 90
url: /net/aspose.tasks/calendarexception/monthposition/
---
## CalendarException.MonthPosition property

Gets or sets the position of a month item within a month.

```csharp
public MonthPosition MonthPosition { get; set; }
```

## Examples

Shows how to define calendar exception by month day.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// create a calendar
var calendar = project.Calendars.Add("Calendar1");

// create calendar exception for every friday
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// check that aa friday is exceptional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// add the exception to the calendar
calendar.Exceptions.Add(exception);
```

### See Also

* enum [MonthPosition](../../monthposition/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


