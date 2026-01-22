---
title: Class WeeklyRepetitionBase
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.WeeklyRepetitionBase class. Represents a base class for repetitions in weekly recurrence pattern
type: docs
weight: 3570
url: /net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

Represents a base class for repetitions in weekly recurrence pattern.

```csharp
public abstract class WeeklyRepetitionBase
```

## Properties

| Name | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Gets or sets a number of weeks which represents the interval in weeks between occurrences. |

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


