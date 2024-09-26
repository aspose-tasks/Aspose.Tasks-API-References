---
title: Enum DayType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DayType enum. Specifies the day of a week
type: docs
weight: 450
url: /net/aspose.tasks/daytype/
---
## DayType enumeration

Specifies the day of a week.

```csharp
public enum DayType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Exception | `0` | Indicates Exception day type. |
| Sunday | `1` | Indicates Sunday day type. |
| Monday | `2` | Indicates Monday day type. |
| Tuesday | `3` | Indicates Tuesday day type. |
| Wednesday | `4` | Indicates Wednesday day type. |
| Thursday | `5` | Indicates Thursday day type. |
| Friday | `6` | Indicates Friday day type. |
| Saturday | `7` | Indicates Saturday day type. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


