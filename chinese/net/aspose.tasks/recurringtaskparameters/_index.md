---
title: "类 RecurringTaskParameters"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RecurringTaskParameters 类。表示用于在项目中创建循环任务的一组参数"
type: docs
weight: 1730
url: /zh/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

表示用于在项目中创建循环任务的一组参数。

```csharp
public class RecurringTaskParameters
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | 初始化 `RecurringTaskParameters` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | 获取或设置循环任务一次出现的持续时间。[`Duration`](./duration/) 类的实例。 |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | 获取或设置一个值，指示是否即使在没有任何资源可用于工作时仍安排循环任务。 |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | 获取或设置循环任务的重复模式。可以是 [`RecurrencePattern`](./recurrencepattern/) 枚举的其中一个值。 |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | 获取或设置循环任务的名称。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | 为循环任务设置日历。该日历从项目日历集合中选择。 |

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


