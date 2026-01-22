---
title: Enum TimeUnitType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TimeUnitType enum. Specifies the type of a time unit
type: docs
weight: 2540
url: /net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Specifies the type of a time unit.

```csharp
public enum TimeUnitType : sbyte
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `-1` | Indicates Undefined value means that the field was not defined in original project file. |
| Minute | `0` | Indicates Minute time unit type. |
| ElapsedMinute | `1` | Indicates Elapsed minute time unit type. |
| Hour | `2` | Indicates Hour time unit type. |
| ElapsedHour | `3` | Indicates Elapsed hour time unit type. |
| Day | `4` | Indicates Day time unit type. |
| ElapsedDay | `5` | Indicates Elapsed day time unit type. |
| Week | `6` | Indicates Week time unit type. |
| ElapsedWeek | `7` | Indicates Elapsed week time unit type. |
| Month | `8` | Indicates Month time unit type. |
| ElapsedMonth | `9` | Indicates Elapsed month time unit type. |
| Percent | `10` | Indicates Percent time unit type. |
| ElapsedPercent | `11` | Indicates Elapsed percent time unit type. |
| Null | `12` | Indicates Null time unit type. |
| MinuteEstimated | `13` | Indicates Minute estimated time unit type. |
| ElapsedMinuteEstimated | `14` | Indicates Elapsed minute estimated time unit type. |
| HourEstimated | `15` | Indicates Hour estimated time unit type. |
| ElapsedHourEstimated | `16` | Indicates Elapsed hour estimated time unit type. |
| DayEstimated | `17` | Indicates Day estimated time unit type. |
| ElapsedDayEstimated | `18` | Indicates Elapsed day estimated time unit type. |
| WeekEstimated | `19` | Indicates Week estimated time unit type. |
| ElapsedWeekEstimated | `20` | Indicates Elapsed week estimated time unit type. |
| MonthEstimated | `21` | Indicates Month estimated time unit type. |
| ElapsedMonthEstimated | `22` | Indicates Elapsed month estimated time unit type. |
| PercentEstimated | `23` | Indicates Percent estimated time unit type. |
| ElapsedPercentEstimated | `24` | Indicates Elapsed percent estimated time unit type. |
| Year | `25` | Indicates Year time unit type. |

## Remarks

While exporting into XML the Undefined values will be eliminated from resulting XML.

## Examples

Shows how to convert a duration into different time unit types.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Get a task to calculate its duration in different formats
var task = project.RootTask.Children.GetById(1);

// Get the duration in Minutes, Days, Hours, Weeks and Months
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


