---
title: "Aspose::Tasks::Calendar class"
linktitle: "Calendar"
articleTitle: "Calendar"
second_title: "Aspose.Tasks for C++"
description: "Represents a calendar used in a project."
type: docs
weight: 10
url: /cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Represents a calendar used in a project.

How to create simple calendar from scratch.

```cpp
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

```cpp
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

Calendars are used to define standard working and non-working times. Projects must have one base calendar. Tasks and resources can have their own non-base calendars that are based on a base calendar.

## Methods

| Name | Description |
| --- | --- |
| [Delete](./delete/) | Removes calendar from project. |
| [Equals](./equals/) | Returns a value indicating whether this instance is equal to a specified object. |
| [get_BaseCalendar](./get_basecalendar/) | Gets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar. |
| [get_Exceptions](./get_exceptions/) | Gets CalendarExceptionCollection object. The collection of exceptions that is associated with the calendar. |
| [get_Guid](./get_guid/) | Gets calendar's Guid. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Gets a value indicating whether the calendar is a base calendar. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Gets a value indicating whether the calendar is a baseline calendar. |
| [get_Name](./get_name/) | Gets the name of the calendar. |
| [get_Uid](./get_uid/) | Gets the unique identifier of the calendar. |
| [get_WeekDays](./get_weekdays/) | Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar. |
| [get_WorkWeeks](./get_workweeks/) | Gets WorkWeekCollections object. The collection of work weeks that is associated with the calendar. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Calculates the date when the specified amount of work time will pass according to the calendar. |
| [GetHashCode](./gethashcode/) | Returns a hash code for the instance of the class. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Gets ICalendar instance which can be used to perform calculations on the intersection of work schedules of 2 calendars. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Calculates next working day start for the specified date. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Calculates the end of the previous working date from the specified date. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Returns start date based on the specified finish date and duration. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Calculates the task finish date and time from its start date, split parts and the work duration. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Returns the amount of working hours at the specified date. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Returns amount of working hours between the specified dates. |
| [GetWorkingTimes](./getworkingtimes/) | Returns WorkingTimeCollection of working times for the specified date. |
| [GetWorkStart](./getworkstart/) | Calculates next working time start beginning from the specified date and time. |
| [IsDayWorking](./isdayworking/) | Determines whether the specified day is a working day according to the calendar. |
| [IsEmpty](./isempty/) | Returns whether the calendar doesn't have working hours defined. |
| [Make24HourCalendar](./make24hourcalendar/) | Makes a given Calendar to be a 24Hour Calendar . 24Hours Calendar is a Calendar in which every day of week is working with Round-the-clock working hours. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Makes a given Calendar as Night Shift Calendar . |
| [MakeStandardCalendar](./makestandardcalendar/) | Creates default standard calendar. |
| [set_BaseCalendar](./set_basecalendar/) | Sets the base calendar on which this calendar depends. Only applicable if the calendar is not a base calendar. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Sets a value indicating whether the calendar is a baseline calendar. |
| [set_Name](./set_name/) | Sets the name of the calendar. |
| [set_Uid](./set_uid/) | Sets the unique identifier of the calendar. |

