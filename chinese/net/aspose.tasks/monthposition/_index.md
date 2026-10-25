---
title: "枚举 MonthPosition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MonthPosition 枚举。指定月份项在月份内的位置"
type: docs
weight: 1070
url: /zh/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

指定月份项在月份中的位置。

```csharp
public enum MonthPosition
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示未定义的月份位置。 |
| First | `0` | 指示第一位置的月份位置。 |
| Second | `1` | 指示第二位置的月份位置。 |
| Third | `2` | 指示第三位置的月份位置。 |
| Fourth | `3` | 指示第四位置的月份位置。 |
| Last | `4` | 指示最后位置的月份位置。 |

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


