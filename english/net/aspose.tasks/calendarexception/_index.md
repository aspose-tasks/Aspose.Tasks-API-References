---
title: Class CalendarException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CalendarException class. Represent exceptional time periods in a calendar
type: docs
weight: 250
url: /net/aspose.tasks/calendarexception/
---
## CalendarException class

Represent exceptional time periods in a calendar.

```csharp
public sealed class CalendarException
```

## Constructors

| Name | Description |
| --- | --- |
| [CalendarException](calendarexception/)() | Initializes a new instance of the `CalendarException` class. |

## Properties

| Name | Description |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Gets the DayTypeCollection for this object. The days of the week on which the exception is valid. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Gets or sets a value indicating whether the specified date or day type is working. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Gets or sets a value indicating whether the range of recurrence is defined by entering a number of occurrences. False specifies that the range of recurrence is defined by entering a finish date. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Gets or sets the beginning of the exception time. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Gets or sets the month for which an exception recurrence is scheduled. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Gets or sets the day of a month on which an exception recurrence is scheduled. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Gets or sets the month item for which an exception recurrence is scheduled. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Gets or sets the position of a month item within a month. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Gets or sets the name of the exception. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Gets or sets the number of occurrences for which the calendar exception is valid. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Gets the parent calendar for this object. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Gets or sets the period of recurrence for the exception. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Gets or sets the end of the exception time. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Gets or sets the exception type. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Gets or sets the WorkingTimeCollection object. The collection of working times that defines the time worked on the weekday.  At least one working time must present, and there can't be more than five. |

## Methods

| Name | Description |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Returns true if the specified instance of the DateTime struct is the exception day. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Deletes the Exception instance from parent calendar CalendarExceptionCollection object. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Returns dates on which the calendar exception is applicable. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Returns the working time for a calendar exception. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


