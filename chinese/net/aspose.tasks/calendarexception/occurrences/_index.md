---
title: "CalendarException.Occurrences"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 属性。获取或设置日历异常有效的出现次数。"
type: docs
weight: 110
url: /zh/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

获取或设置日历异常有效的出现次数。

```csharp
public int Occurrences { get; set; }
```

## 示例

展示如何通过出现次数定义日历例外。

```csharp
var project = new Project();

// 定义日历
var calendar = project.Calendars.Add("Calendar1");

// 定义例外并指定出现次数
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// 向日历添加例外
calendar.Exceptions.Add(exception);
```

### 另见

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


