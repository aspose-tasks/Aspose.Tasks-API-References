---
title: RecurringTaskParameters.RecurrencePattern
second_title: Aspose.Tasks for .NET API Reference
description: RecurringTaskParameters property. Gets or sets the recurrence pattern of the recurring task. Can be one of the values of RecurrencePattern enumeration
type: docs
weight: 40
url: /net/aspose.tasks/recurringtaskparameters/recurrencepattern/
---
## RecurringTaskParameters.RecurrencePattern property

Gets or sets the recurrence pattern of the recurring task. Can be one of the values of `RecurrencePattern` enumeration.

```csharp
public RecurrencePatternBase RecurrencePattern { get; set; }
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

* class [RecurrencePatternBase](../../recurrencepatternbase/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


