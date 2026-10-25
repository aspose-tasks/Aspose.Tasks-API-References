---
title: "类 DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.DailyWorkRepetition 类。表示用于基于工作日的每日重复模式的类"
type: docs
weight: 420
url: /zh/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

表示基于工作日的每日重复模式的类。

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | 初始化 `DailyWorkRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示发生间隔天数的天数。 |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


