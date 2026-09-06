---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取此日历的 WeekDaysCollection。定义日历的工作日集合。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

获取此日历的 WeekDaysCollection。定义该日历的工作日集合。

```csharp
public WeekDayCollection WeekDays { get; }
```

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

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


