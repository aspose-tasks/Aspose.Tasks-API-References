---
title: "类 ByMonthDayRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ByMonthDayRepetition 类。表示基于月份中某一天的绝对位置的模式"
type: docs
weight: 170
url: /zh/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

表示基于月份中某天绝对位置的模式。

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | 初始化 `ByMonthDayRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | 获取或设置任务必须重复的月份中某一天的位置。 |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示两次出现之间间隔月份数的月份数。 |

## 示例

展示如何在创建新循环任务时使用月份天数重复。

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


