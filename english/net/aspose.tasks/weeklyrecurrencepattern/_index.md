---
title: Class WeeklyRecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeeklyRecurrencePattern class. Represents the set of parameters are used to create a weekly recurring task in a project
type: docs
weight: 3550
url: /net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Represents the set of parameters are used to create a weekly recurring task in a project.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Name | Description |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Initializes a new instance of the `WeeklyRecurrencePattern` class. |

## Properties

| Name | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Gets or sets the recurrence range. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Gets or sets the recurring repetition pattern. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


