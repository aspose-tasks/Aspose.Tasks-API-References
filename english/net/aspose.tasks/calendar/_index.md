---
title: Calendar
second_title: Aspose.Tasks for .NET API Reference
description: Represents a calendar used in a project.
type: docs
weight: 230
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
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar) { get; set; } | Gets or sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar. |
| [Exceptions](../../aspose.tasks/calendar/exceptions) { get; } | Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar. |
| [Guid](../../aspose.tasks/calendar/guid) { get; } | Gets or sets calendar's Guid. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar) { get; } | Gets a value indicating whether the calendar is a base calendar. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar) { get; set; } | Gets or sets a value indicating whether the calendar is a baseline calendar. |
| [Name](../../aspose.tasks/calendar/name) { get; set; } | Gets or sets the name of the calendar. |
| [Uid](../../aspose.tasks/calendar/uid) { get; set; } | Gets or sets the unique identifier of the calendar. |
| [WeekDays](../../aspose.tasks/calendar/weekdays) { get; } | Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks) { get; } | Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar. |

## Methods

| Name | Description |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar)(Calendar) | Makes a given Calendar to be a 24Hour Calendar. 24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar)(Calendar) | Makes a given Calendar as Night Shift Calendar. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar)(Calendar) | Creates default standard calendar. |
| [Delete](../../aspose.tasks/calendar/delete)() | Removes calendar from project. |
| override [Equals](../../aspose.tasks/calendar/equals)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork)(DateTime, Duration) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode)() | Returns a hash code for the instance of the class. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart)(DateTime) | Calculates next working day start from the date. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend)(DateTime) | Calculates previous working date end from the specified date. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration)(DateTime, Duration) | Returns StartDate based on specified FinishDate and Duration. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Returns StartDate based on specified FinishDate and Duration. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration)(Task, TimeSpan) | Calculates the task finish date and time from its start date, split parts and the duration. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours_1)(DateTime) | Returns amount of working hours at the date. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours)(DateTime, DateTime) | Return working hours for the specified dates. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes)(DateTime) | Returns [`WorkingTimeCollection`](../workingtimecollection) of working times for the specified date. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking)(DateTime) | Determines whether the day is working day. |

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

Shows how to define a new calendar, add week days to it and define working times for days.

```csharp
var project = new Project();

// Define a calendar
var calendar = project.Calendars.Add("Calendar1");

// Add working days monday through thursday with default timings
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Set friday as short working day
var weekDay = new WeekDay(DayType.Friday);

// Sets working time. Only time part of DateTime is important
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// working with the project...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
