---
title: Class DailyRepetitionBase
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.DailyRepetitionBase class. Represents a base class for repetitions in daily recurrence pattern
type: docs
weight: 410
url: /net/aspose.tasks/dailyrepetitionbase/
---
## DailyRepetitionBase class

Represents a base class for repetitions in daily recurrence pattern.

```csharp
public abstract class DailyRepetitionBase
```

## Properties

| Name | Description |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Gets or sets a number of days which represents the interval in days between occurrences. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


