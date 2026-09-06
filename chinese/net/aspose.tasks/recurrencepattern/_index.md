---
title: "枚举 RecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RecurrencePattern 枚举。表示循环任务的重复模式类型"
type: docs
weight: 1690
url: /zh/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

表示循环任务的重复模式类型。

```csharp
[Flags]
public enum RecurrencePattern
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Daily | `1` | 每日模式。 |
| Weekly | `4` | 每周模式。 |
| Monthly | `8` | 每月模式。 |
| Yearly | `10` | 每年模式。 |

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


