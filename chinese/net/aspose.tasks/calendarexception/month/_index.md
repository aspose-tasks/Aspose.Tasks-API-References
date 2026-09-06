---
title: "CalendarException.Month"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 属性。获取或设置异常重复计划的月份。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/calendarexception/month/
---
## CalendarException.Month property

获取或设置异常重复计划的月份。

```csharp
public Month Month { get; set; }
```

## 示例

展示如何按月份日期定义日历异常。

```csharp
var project = new Project(DataDir + "project_test.mpp");

// 创建日历
var calendar = project.Calendars.Add("Calendar1");

// 为每个星期五创建日历异常
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// 检查星期五是否为例外
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// 将异常添加到日历中
calendar.Exceptions.Add(exception);
```

### 另见

* enum [Month](../../month/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


