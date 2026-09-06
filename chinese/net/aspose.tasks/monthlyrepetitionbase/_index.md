---
title: "类 MonthlyRepetitionBase"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MonthlyRepetitionBase 类。表示每月日期位置的基础模式"
type: docs
weight: 1090
url: /zh/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

表示月度日期位置的基础模式。

```csharp
public abstract class MonthlyRepetitionBase
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示两次出现之间间隔月份数的月份数。 |

## 示例

展示在创建循环任务时如何使用月度重复模式的重复。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


