---
title: "类 EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.EndAfterRecurrenceRange 类。表示受出现次数限制的循环任务的重复范围"
type: docs
weight: 500
url: /zh/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

表示受出现次数限制的循环任务的重复范围。

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | 初始化 `EndAfterRecurrenceRange` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | 获取或设置限制循环任务重复范围的出现次数。 |
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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


