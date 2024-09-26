---
title: EndAfterRecurrenceRange.OccurrenceNumber
second_title: Aspose.Tasks for .NET API Reference
description: EndAfterRecurrenceRange property. Gets or sets the number of occurrences which limits the recurrence range of the recurring task
type: docs
weight: 20
url: /net/aspose.tasks/endafterrecurrencerange/occurrencenumber/
---
## EndAfterRecurrenceRange.OccurrenceNumber property

Gets or sets the number of occurrences which limits the recurrence range of the recurring task.

```csharp
public int OccurrenceNumber { get; set; }
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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


