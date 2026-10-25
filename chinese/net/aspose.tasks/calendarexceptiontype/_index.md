---
title: "枚举 CalendarExceptionType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalendarExceptionType 枚举。指定日历异常类型"
type: docs
weight: 270
url: /zh/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

指定日历例外类型。

```csharp
public enum CalendarExceptionType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Daily | `0` | 表示每日异常类型。 |
| YearlyByDay | `1` | 表示按月份天数的年度异常类型。 |
| YearlyByPosition | `2` | 表示按位置的年度异常类型。 |
| MonthlyByDay | `3` | 表示按月份天数的月度异常类型。 |
| MonthlyByPosition | `4` | 表示按位置的月度异常类型。 |
| Weekly | `5` | 指示每周例外类型。 |
| ByDayCount | `6` | 指示按天计数的例外类型。 |
| ByWeekDayCount | `7` | 指示按工作日计数的例外类型。 |
| NoExceptionType | `8` | 指示无例外类型。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


