---
title: Class CalendarExceptionCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CalendarExceptionCollection class. Represents a collection of CalendarException objects
type: docs
weight: 260
url: /net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Represents a collection of [`CalendarException`](../calendarexception/) objects.

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Gets the number of objects contained in this `CalendarExceptionCollection` object. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Gets the parent calendar for this object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Adds CalendarException instance to this collection object. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Adds range of exceptions to the internal list. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Removes all items from the `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Removes [`CalendarException`](../calendarexception/) instance from this collection. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Converts the CalendarExceptionCollection object to a list of [`CalendarException`](../calendarexception/) objects. |

## Examples

Shows how to use calendar exception collection to define calendar exceptions.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// remove all exceptions
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### See Also

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


