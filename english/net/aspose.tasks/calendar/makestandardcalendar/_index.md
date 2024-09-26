---
title: Calendar.MakeStandardCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Calendar method. Creates default standard calendar
type: docs
weight: 30
url: /net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Creates default standard calendar.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calendar | Calendar | Calendar to make standard calendar from. |

### Return Value

Calendar with 5 working days (Monday-Friday) with working times 8-12 and 13-17.

## Examples

Shows how to create a standard calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// show working hours
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Shows how to create a calendar with exception days.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Update the calendar information
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


