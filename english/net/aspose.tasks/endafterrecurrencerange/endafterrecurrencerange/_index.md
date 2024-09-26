---
title: EndAfterRecurrenceRange.EndAfterRecurrenceRange
second_title: Aspose.Tasks for .NET API Reference
description: EndAfterRecurrenceRange constructor. Initializes a new instance of the EndAfterRecurrenceRange class
type: docs
weight: 10
url: /net/aspose.tasks/endafterrecurrencerange/endafterrecurrencerange/
---
## EndAfterRecurrenceRange constructor

Initializes a new instance of the [`EndAfterRecurrenceRange`](../) class.

```csharp
public EndAfterRecurrenceRange()
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


