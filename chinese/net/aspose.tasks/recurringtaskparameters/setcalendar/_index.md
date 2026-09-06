---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "RecurringTaskParameters 方法。为循环任务设置日历。该日历从项目日历集合中选择"
type: docs
weight: 60
url: /zh/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

为循环任务设置日历。该日历从项目日历集合中选择。

```csharp
public void SetCalendar(Project project, string calendarName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| project | Project | 具有日历集合的项目。 |
| calendarName | 字符串 | 日历的名称。 |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


