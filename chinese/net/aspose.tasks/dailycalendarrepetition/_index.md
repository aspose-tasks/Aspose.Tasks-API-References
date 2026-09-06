---
title: "类 DailyCalendarRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DailyCalendarRepetition 类。表示基于日历天数的每日重复模式中的重复类"
type: docs
weight: 390
url: /zh/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

表示基于日历天的每日重复模式的类。

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | 初始化 `DailyCalendarRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示发生间隔天数的天数。 |

## 示例

展示如何在创建循环任务时使用每日工作重复模式的重复以及“24 小时”。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// 进一步处理项目...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


