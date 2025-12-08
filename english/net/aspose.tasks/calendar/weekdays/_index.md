---
title: Calendar.WeekDays
second_title: Aspose.Tasks for .NET API Reference
description: Calendar property. Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar
type: docs
weight: 120
url: /net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Gets WeekDaysCollection for this calendar. The collection of weekdays that defines the calendar.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Examples

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


