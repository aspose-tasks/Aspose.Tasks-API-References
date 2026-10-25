---
title: "EndAfterRecurrenceRange.EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET API 参考"
description: "EndAfterRecurrenceRange 构造函数。初始化 EndAfterRecurrenceRange 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/endafterrecurrencerange/endafterrecurrencerange/
---
## EndAfterRecurrenceRange constructor

初始化 [`EndAfterRecurrenceRange`](../) 类的新实例。

```csharp
public EndAfterRecurrenceRange()
```

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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


