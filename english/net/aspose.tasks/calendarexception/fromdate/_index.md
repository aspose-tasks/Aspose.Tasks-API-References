---
title: CalendarException.FromDate
second_title: Aspose.Tasks for .NET API Reference
description: CalendarException property. Gets or sets the beginning of the exception time
type: docs
weight: 50
url: /net/aspose.tasks/calendarexception/fromdate/
---
## CalendarException.FromDate property

Gets or sets the beginning of the exception time.

```csharp
public DateTime FromDate { get; set; }
```

## Examples

Shows how to add/remove calendar exceptions.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// create a calendar
var calendar = project.Calendars.Add("Calendar1");

// create week days exception for a holiday
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// check that date is exceptional
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// remove an exception
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// add an exception
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// print exceptions
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### See Also

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


