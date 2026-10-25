---
title: "CalendarException.EnteredByOccurrences"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 属性。获取或设置一个值，指示是否通过输入出现次数的数量来定义重复范围。False 指定通过输入结束日期来定义重复范围。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

获取或设置一个值，指示是否通过输入出现次数来定义重复范围。False 表示通过输入结束日期来定义重复范围。

```csharp
public bool EnteredByOccurrences { get; set; }
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


