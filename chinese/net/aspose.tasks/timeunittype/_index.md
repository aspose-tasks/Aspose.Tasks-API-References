---
title: "枚举 TimeUnitType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TimeUnitType 枚举。指定时间单位的类型"
type: docs
weight: 2570
url: /zh/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

指定时间单位的类型。

```csharp
public enum TimeUnitType : sbyte
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示未定义的值意味着该字段在原始项目文件中未定义。 |
| Minute | `0` | 指示分钟时间单位类型。 |
| ElapsedMinute | `1` | 指示已用分钟时间单位类型。 |
| Hour | `2` | 指示小时时间单位类型。 |
| ElapsedHour | `3` | 指示已用小时时间单位类型。 |
| Day | `4` | 指示天时间单位类型。 |
| ElapsedDay | `5` | 指示已用天时间单位类型。 |
| Week | `6` | 指示周时间单位类型。 |
| ElapsedWeek | `7` | 指示已用周时间单位类型。 |
| Month | `8` | 指示月时间单位类型。 |
| ElapsedMonth | `9` | 指示已用月时间单位类型。 |
| Percent | `10` | 指示百分比时间单位类型。 |
| ElapsedPercent | `11` | 指示已用百分比时间单位类型。 |
| Null | `12` | 指示空时间单位类型。 |
| MinuteEstimated | `13` | 指示分钟估计时间单位类型。 |
| ElapsedMinuteEstimated | `14` | 指示已用分钟估计时间单位类型。 |
| HourEstimated | `15` | 指示小时估计时间单位类型。 |
| ElapsedHourEstimated | `16` | 指示已用小时估计时间单位类型。 |
| DayEstimated | `17` | 指示天估计时间单位类型。 |
| ElapsedDayEstimated | `18` | 指示已用天估计时间单位类型。 |
| WeekEstimated | `19` | 指示周估计时间单位类型。 |
| ElapsedWeekEstimated | `20` | 指示已用周估计时间单位类型。 |
| MonthEstimated | `21` | 指示月估计时间单位类型。 |
| ElapsedMonthEstimated | `22` | 指示已用月估计时间单位类型。 |
| PercentEstimated | `23` | 指示百分比估计时间单位类型。 |
| ElapsedPercentEstimated | `24` | 指示已过去的百分比估计时间单位类型。 |
| Year | `25` | 指示年份时间单位类型。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何将持续时间转换为不同的时间单位类型。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 获取任务以计算其持续时间的不同格式
var task = project.RootTask.Children.GetById(1);

// 获取以分钟、天、小时、周和月为单位的持续时间
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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


