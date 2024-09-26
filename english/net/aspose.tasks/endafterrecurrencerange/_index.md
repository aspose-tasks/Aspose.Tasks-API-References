---
title: Class EndAfterRecurrenceRange
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.EndAfterRecurrenceRange class. Represents the recurrence range of recurring task which is limited by occurrence number
type: docs
weight: 500
url: /net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Represents the recurrence range of recurring task which is limited by occurrence number.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Constructors

| Name | Description |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Initializes a new instance of the `EndAfterRecurrenceRange` class. |

## Properties

| Name | Description |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Gets or sets the number of occurrences which limits the recurrence range of the recurring task. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Gets or sets the start date of the recurrence range of the recurring task. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


