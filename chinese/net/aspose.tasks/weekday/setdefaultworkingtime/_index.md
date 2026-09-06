---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WeekDay 方法。为指定的星期几设置默认时间段"
type: docs
weight: 130
url: /zh/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

为指定的工作日设置默认时间段。

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 天 | WeekDay | 用于设置默认工作日的星期。 |

## 示例

展示如何为一天设置默认工作时间。

```csharp
var project = new Project();

// 定义日历
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// 添加从周一到周四的工作日，使用默认时间安排
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// 让我们打印所有工作时间
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### 另见

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


