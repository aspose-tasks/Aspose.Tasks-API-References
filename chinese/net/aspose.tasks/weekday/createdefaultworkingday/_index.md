---
title: "WeekDay.CreateDefaultWorkingDay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WeekDay 方法。创建默认工作日。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/weekday/createdefaultworkingday/
---
## WeekDay.CreateDefaultWorkingDay method

创建默认工作日。

```csharp
public static WeekDay CreateDefaultWorkingDay(DayType dayType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dayType | DayType | 用于创建默认工作日的星期类型。 |

### 返回值

一个默认工作日，工作时间为 8-12 和 13-17。

## 示例

展示如何通过定义工作日来创建新日历。

```csharp
var project = new Project();

// 定义日历
var calendar = project.Calendars.Add("Calendar1");

// 添加从周一到周四的工作日，使用默认时间安排
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// 检查例外日的起始和结束日期
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// 将周五设为短工作日

// 设置工作时间。 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// 有一种方法可以将 <see cref=\"DayOfWeek\" /> 转换为 <see cref=\"Aspose.Tasks.DayType\" />。
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


