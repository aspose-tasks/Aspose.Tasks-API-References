---
title: "类 CalendarException"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalendarException 类。表示日历中的异常时间段"
type: docs
weight: 250
url: /zh/net/aspose.tasks/calendarexception/
---
## CalendarException class

表示日历中的特殊时间段。

```csharp
public sealed class CalendarException
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CalendarException](calendarexception/)() | 初始化 `CalendarException` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | 获取此对象的 DayTypeCollection。异常有效的星期几。 |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | 获取或设置一个值，指示指定的日期或天类型是否为工作日。 |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | 获取或设置一个值，指示是否通过输入出现次数来定义重复范围。False 表示通过输入结束日期来定义重复范围。 |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | 获取或设置异常时间的开始。 |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | 获取或设置异常重复计划的月份。 |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | 获取或设置异常重复计划的月份中的日期。 |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | 获取或设置异常重复计划的月份项。 |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | 获取或设置月份项在月份中的位置。 |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | 获取或设置异常的名称。 |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | 获取或设置日历异常有效的出现次数。 |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | 获取此对象的父日历。 |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | 获取或设置异常的重复周期。 |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | 获取或设置异常时间的结束。 |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | 获取或设置异常类型。 |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | 获取或设置 WorkingTimeCollection 对象。该集合定义了工作日的工作时间。必须至少存在一个工作时间，且不能超过五个。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | 如果指定的 DateTime 结构实例是例外日，则返回 true。 |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | 从父日历 CalendarExceptionCollection 对象中删除 Exception 实例。 |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | 返回日历例外适用的日期。 |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | 返回日历例外的工作时间。 |

## 示例

展示如何添加/删除日历例外。

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 创建日历
var calendar = project.Calendars.Add("Calendar1");

// 为假期创建工作日例外
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// 检查日期是否为例外
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// 删除一个例外
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// 添加一个例外
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// 打印例外
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


