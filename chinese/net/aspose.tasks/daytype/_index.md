---
title: "枚举 DayType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DayType 枚举。指定一周中的某天"
type: docs
weight: 450
url: /zh/net/aspose.tasks/daytype/
---
## DayType enumeration

指定一周中的天。

```csharp
public enum DayType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Exception | `0` | 指示例外日类型。 |
| Sunday | `1` | 指示星期日类型。 |
| Monday | `2` | 指示星期一类型。 |
| Tuesday | `3` | 指示星期二类型。 |
| Wednesday | `4` | 指示星期三类型。 |
| Thursday | `5` | 指示星期四类型。 |
| Friday | `6` | 指示星期五类型。 |
| Saturday | `7` | 指示星期六类型。 |

## 示例

展示如何定义新日历、向其添加工作日并为这些天定义工作时间。

```csharp
var project = new Project();

// 定义日历
var calendar = project.Calendars.Add("Calendar1");

// 添加从周一到周四的工作日，使用默认时间安排
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// 将周五设为短工作日
var weekDay = new WeekDay(DayType.Friday);

// 设置工作时间。仅 DateTime 的时间部分重要。
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// 正在处理项目……
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


