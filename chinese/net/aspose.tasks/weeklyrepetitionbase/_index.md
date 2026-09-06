---
title: "类 WeeklyRepetitionBase"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeeklyRepetitionBase 类。表示每周重复模式中重复的基类。"
type: docs
weight: 3600
url: /zh/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

表示每周循环模式中重复的基类。

```csharp
public abstract class WeeklyRepetitionBase
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示发生间隔（以周为单位）的周数。 |

## 示例

展示如何创建循环任务。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


