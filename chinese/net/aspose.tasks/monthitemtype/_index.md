---
title: "枚举 MonthItemType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MonthItemType 枚举。指定为其安排异常重复的月份项"
type: docs
weight: 1050
url: /zh/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

指定为其安排异常重复的月份项。

```csharp
public enum MonthItemType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 表示未定义的月份项类型。 |
| Day | `0` | 表示日期月份项类型。 |
| Weekday | `1` | 表示工作日月份项类型。 |
| WeekendDay | `2` | 表示周末日月份项类型。 |
| Sunday | `3` | 表示星期日月份项类型。 |
| Monday | `4` | 表示星期一月份项类型。 |
| Tuesday | `5` | 表示星期二月份项类型。 |
| Wednesday | `6` | 表示星期三月份项类型。 |
| Thursday | `7` | 表示星期四月份项类型。 |
| Friday | `8` | 表示星期五月份项类型。 |
| Saturday | `9` | 表示星期六月份项类型。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


