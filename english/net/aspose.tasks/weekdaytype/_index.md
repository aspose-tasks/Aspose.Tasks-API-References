---
title: Enum WeekdayType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeekdayType enum. Represents a weekday of a project in the instance of RecurringTaskInfo class
type: docs
weight: 3540
url: /net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Represents a weekday of a project in the instance of [`RecurringTaskInfo`](../recurringtaskinfo/) class.

```csharp
[Flags]
public enum WeekdayType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Indicates None weekday type. |
| Sunday | `1` | Indicates Sunday weekday type. |
| Monday | `2` | Indicates Monday weekday type. |
| Tuesday | `4` | Indicates Tuesday weekday type. |
| Wednesday | `8` | Indicates Wednesday weekday type. |
| Thursday | `10` | Indicates Thursday weekday type. |
| Friday | `20` | Indicates Friday weekday type. |
| Saturday | `40` | Indicates Saturday weekday type. |

## Examples

Shows how to create a recurring task.

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

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


