---
title: "类 DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DailyRecurrencePattern 类。表示用于在项目中创建每日循环任务的一组参数。"
type: docs
weight: 400
url: /zh/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

表示用于在项目中创建每日循环任务的参数集。

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | 初始化 `DailyRecurrencePattern` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 获取或设置循环范围。 |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | 获取或设置每日循环模式中的重复模式。 |

## 示例

展示在创建循环任务时如何使用每日工作重复模式的重复。

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// 进一步处理项目...
// ...
```

### 另见

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


