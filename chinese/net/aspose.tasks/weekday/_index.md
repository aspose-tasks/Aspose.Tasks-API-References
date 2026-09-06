---
title: "类 WeekDay"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeekDay 类。表示一周中的工作日，可定义常规工作日或日历中的例外日。"
type: docs
weight: 3540
url: /zh/net/aspose.tasks/weekday/
---
## WeekDay class

表示一个工作日，可定义一周的常规天数或日历中的例外天数。

```csharp
public class WeekDay
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WeekDay](weekday/#constructor)() | 初始化 `WeekDay` 类的新实例。 |
| [WeekDay](weekday/#constructor_1)(DayType) | 使用指定的天类型初始化 `WeekDay` 类的新实例。 |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | 使用指定的天类型和工作时间段列表初始化 `WeekDay` 类的新实例。 |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | 使用指定的天类型和工作时间段初始化 `WeekDay` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | 获取一天的类型。 |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | 获取或设置一个值，指示指定的日期或天类型是否为工作日。 |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | 获取或设置例外时间的开始。 |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | 获取或设置例外时间的结束。 |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | 获取此 WeekDay 实例的 WorkingTimeCollection。该集合包含定义工作日工作时间的工作时间段。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | 创建默认工作日。 |
| [Clone](../../aspose.tasks/weekday/clone/)() | 返回该工作日的深拷贝。 |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | 返回 `WeekDay` 类实例的哈希码值。 |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | 返回工作日的工作时间。 |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | 将 .Net 的 DayOfWeek 强制转换为 [`DayType`](./daytype/)。 |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | 为指定的工作日设置默认时间段。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


