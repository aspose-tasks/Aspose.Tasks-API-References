---
title: "CalendarException.DaysOfWeek"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 属性。获取此对象的 DayTypeCollection。异常有效的星期几。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

获取此对象的 DayTypeCollection。异常有效的星期几。

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## 示例

展示如何按星期几定义日历异常。

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 创建日历
var calendar = project.Calendars.Add("Calendar1");

// 为每个星期五创建日历异常
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// 检查星期五是否为例外。
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// 将异常添加到日历中
calendar.Exceptions.Add(exception);
```

### 另见

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


