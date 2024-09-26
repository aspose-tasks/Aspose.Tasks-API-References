---
title: Class EndByRecurrenceRange
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.EndByRecurrenceRange class. Represents the recurrence range of recurring task which is limited by finish day
type: docs
weight: 510
url: /net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Represents the recurrence range of recurring task which is limited by finish day.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Constructors

| Name | Description |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Initializes a new instance of the `EndByRecurrenceRange` class. |

## Properties

| Name | Description |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Gets or sets the date which limits the recurrence range of the recurring task. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Gets or sets the start date of the recurrence range of the recurring task. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


