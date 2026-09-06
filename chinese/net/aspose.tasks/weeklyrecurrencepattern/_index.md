---
title: "类 WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeeklyRecurrencePattern 类。表示用于在项目中创建每周重复任务的一组参数。"
type: docs
weight: 3580
url: /zh/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

表示用于在项目中创建每周循环任务的参数集合。

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | 初始化 `WeeklyRecurrencePattern` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | 获取或设置循环范围。 |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | 获取或设置循环重复模式。 |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


