---
title: "枚举 WeekdayType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WeekdayType 枚举。表示项目中 RecurringTaskInfo 类实例的工作日"
type: docs
weight: 3570
url: /zh/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

表示项目中 [`RecurringTaskInfo`](../recurringtaskinfo/) 类实例的工作日。

```csharp
[Flags]
public enum WeekdayType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 指示无工作日类型。 |
| Sunday | `1` | 指示星期日工作日类型。 |
| Monday | `2` | 指示星期一工作日类型。 |
| Tuesday | `4` | 指示星期二工作日类型。 |
| Wednesday | `8` | 指示星期三工作日类型。 |
| Thursday | `10` | 指示星期四工作日类型。 |
| Friday | `20` | 指示星期五工作日类型。 |
| Saturday | `40` | 指示星期六工作日类型。 |

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


