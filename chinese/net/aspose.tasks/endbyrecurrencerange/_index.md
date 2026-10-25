---
title: "类 EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.EndByRecurrenceRange 类。表示受完成日期限制的循环任务的重复范围。"
type: docs
weight: 510
url: /zh/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

表示受完成日期限制的循环任务的重复范围。

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | 初始化 `EndByRecurrenceRange` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | 获取或设置限制循环任务重复范围的日期。 |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | 获取或设置循环任务重复范围的开始日期。 |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


