---
title: "类 CalendarExceptionCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalendarExceptionCollection 类。表示 CalendarException 对象的集合"
type: docs
weight: 260
url: /zh/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

表示一个集合 [`CalendarException`](../calendarexception/) 对象。

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | 获取此 `CalendarExceptionCollection` 对象中包含的对象数量。 |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | 返回指定索引处的元素。 |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | 获取此对象的父日历。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | 向此集合对象添加 CalendarException 实例。 |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | 向内部列表添加异常范围。 |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | 从 `CalendarExceptionCollection` 中移除所有项。 |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | 从此集合中移除 [`CalendarException`](../calendarexception/) 实例。 |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | 将 CalendarExceptionCollection 对象转换为 [`CalendarException`](../calendarexception/) 对象的列表。 |

## 示例

展示如何使用日历异常集合来定义日历异常。

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// 移除所有异常
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### 另见

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


