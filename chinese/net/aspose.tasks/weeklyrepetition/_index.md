---
title: "类 WeeklyRepetition"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeeklyRepetition 类。表示一种基于工作日的模式。"
type: docs
weight: 3590
url: /zh/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

表示基于工作日的模式。

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | 初始化 `WeeklyRepetition` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | 获取或设置表示发生间隔（以周为单位）的周数。 |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | 获取或设置工作日的类型。 |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


