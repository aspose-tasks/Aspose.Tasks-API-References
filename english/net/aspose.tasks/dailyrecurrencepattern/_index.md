---
title: Class DailyRecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DailyRecurrencePattern class. Represents the set of parameters are used to create a daily recurring task in a project
type: docs
weight: 400
url: /net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Represents the set of parameters are used to create a daily recurring task in a project.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Name | Description |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Initializes a new instance of the `DailyRecurrencePattern` class. |

## Properties

| Name | Description |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Gets or sets the recurrence range. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Gets or sets the pattern of repetitions in daily recurrence pattern. |

## Examples

Shows how to work with daily work repetition pattern repetitions while create recurring tasks.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// work with the project further...
// ...
```

### See Also

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


