---
title: Enum RecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RecurrencePattern enum. Represents a type of recurrence pattern of a recurrent task
type: docs
weight: 1670
url: /net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Represents a type of recurrence pattern of a recurrent task.

```csharp
[Flags]
public enum RecurrencePattern
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Daily | `1` | Daily pattern. |
| Weekly | `4` | Weekly pattern. |
| Monthly | `8` | Monthly pattern. |
| Yearly | `10` | Yearly pattern. |

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


