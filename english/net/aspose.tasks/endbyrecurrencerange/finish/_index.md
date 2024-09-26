---
title: EndByRecurrenceRange.Finish
second_title: Aspose.Tasks for .NET API Reference
description: EndByRecurrenceRange property. Gets or sets the date which limits the recurrence range of the recurring task
type: docs
weight: 20
url: /net/aspose.tasks/endbyrecurrencerange/finish/
---
## EndByRecurrenceRange.Finish property

Gets or sets the date which limits the recurrence range of the recurring task.

```csharp
public DateTime Finish { get; set; }
```

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

* class [EndByRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endbyrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


