---
title: "类 RecurrenceRangeBase"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RecurrenceRangeBase 类。表示循环任务的重复范围。"
type: docs
weight: 1710
url: /zh/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

表示循环任务的循环范围。

```csharp
public abstract class RecurrenceRangeBase
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | 获取或设置循环任务重复范围的开始日期。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


