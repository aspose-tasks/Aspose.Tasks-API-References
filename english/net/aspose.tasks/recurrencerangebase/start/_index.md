---
title: RecurrenceRangeBase.Start
second_title: Aspose.Tasks for .NET API Reference
description: RecurrenceRangeBase property. Gets or sets the start date of the recurrence range of the recurring task
type: docs
weight: 10
url: /net/aspose.tasks/recurrencerangebase/start/
---
## RecurrenceRangeBase.Start property

Gets or sets the start date of the recurrence range of the recurring task.

```csharp
public DateTime Start { get; set; }
```

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

* class [RecurrenceRangeBase](../)
* namespace [Aspose.Tasks](../../recurrencerangebase/)
* assembly [Aspose.Tasks](../../../)


