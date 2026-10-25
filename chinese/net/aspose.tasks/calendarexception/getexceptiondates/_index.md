---
title: "CalendarException.GetExceptionDates"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 方法。返回日历异常适用的日期"
type: docs
weight: 190
url: /zh/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

返回日历例外适用的日期。

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### 返回值

返回日历异常适用的异常日期集合。

## 示例

展示如何获取特定日历异常生效的日期。

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### 另见

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


