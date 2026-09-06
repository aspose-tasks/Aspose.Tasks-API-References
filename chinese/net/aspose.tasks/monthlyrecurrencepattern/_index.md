---
title: "类 MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.MonthlyRecurrencePattern 类。表示用于在项目中创建月度循环任务的一组参数。"
type: docs
weight: 1080
url: /zh/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

表示用于在项目中创建月度循环任务的参数集。

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | 初始化 `MonthlyRecurrencePattern` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 获取或设置循环范围。 |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | 获取或设置循环重复模式。 |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


