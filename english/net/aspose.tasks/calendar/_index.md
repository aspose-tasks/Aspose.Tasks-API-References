---
title: Calendar
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 220
url: /net/aspose.tasks/calendar/
---
## Calendar class

Represents a calendar used in a project.

```csharp
public class Calendar
```

## Properties

| Name | Description |
| --- | --- |
| [BaseCalendar](basecalendar) { get; set; } | Gets or sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar. Read/write [`Calendar`](../calendar). |
| [Exceptions](exceptions) { get; } | Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar. |
| [IsBaseCalendar](isbasecalendar) { get; } | Gets a value indicating whether the calendar is a base calendar. Read-only Boolean. |
| [IsBaselineCalendar](isbaselinecalendar) { get; set; } | Gets or sets a value indicating whether the calendar is a baseline calendar. Read/write Boolean. |
| [Name](name) { get; set; } | Gets or sets the name of the calendar. Read/write String. |
| [ParentProject](parentproject) { get; } | Gets parent project for this calendar. |
| [Uid](uid) { get; set; } | Gets or sets the unique identifier of the calendar. Read/write Int32. |
| [WeekDays](weekdays) { get; } | Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar. |
| [WorkWeeks](workweeks) { get; } | Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar. |

## Methods

| Name | Description |
| --- | --- |
| static [Make24HourCalendar](make24hourcalendar)(Calendar) | Makes a given Calendar to be a 24Hour Calendar. 24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours. |
| static [MakeNightShiftCalendar](makenightshiftcalendar)(Calendar) | Makes a given Calendar as Night Shift Calendar. |
| static [MakeStandardCalendar](makestandardcalendar)(Calendar) | Creates default standard calendar. |
| [Delete](delete)() | Removes calendar from project. |
| override [Equals](equals)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [GetFinishDateByStartAndWork](getfinishdatebystartandwork)(DateTime, Duration) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [GetFinishDateByStartAndWork](getfinishdatebystartandwork)(DateTime, TimeSpan) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| override [GetHashCode](gethashcode)() | Returns a hash code for the instance of the [`Calendar`](../calendar) class. |
| [GetNextWorkingDayStart](getnextworkingdaystart)(DateTime) | Calculates next working day start from the date. |
| [GetPreviousWorkingDayEnd](getpreviousworkingdayend)(DateTime) | Calculates previous working date end from the specified date. |
| [GetStartDateFromFinishAndDuration](getstartdatefromfinishandduration)(DateTime, Duration) | Returns StartDate based on specified FinishDate and Duration. |
| [GetStartDateFromFinishAndDuration](getstartdatefromfinishandduration)(DateTime, TimeSpan) | Returns StartDate based on specified FinishDate and Duration. |
| [GetTaskFinishDateFromDuration](gettaskfinishdatefromduration)(Task, TimeSpan) | Calculates the task finish date and time from its start date, split parts and the duration. |
| [GetWorkingHours](getworkinghours)(DateTime) | Returns amount of working hours at the date. |
| [GetWorkingHours](getworkinghours)(DateTime, DateTime) | Return working hours for the specified dates. |
| [GetWorkingTimes](getworkingtimes)(DateTime) | Returns [`WorkingTimeCollection`](../workingtimecollection) of working times. |
| [IsDayWorking](isdayworking)(DateTime) | Determines whether the day is working day. |

### Remarks

Calendars are used to define standard working and non-working times. Projects must have one base calendar. Tasks and resources can have their own non-base calendars that are based on a base calendar.

### Examples

How to create simple calendar from scratch.

```csharp
[C#]
// create empty calendar
Calendar calendar = new Calendar("New calendar");
// adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// create new new working day
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Sets working time. Only time part of DateTime is important
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// adds weekend
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
