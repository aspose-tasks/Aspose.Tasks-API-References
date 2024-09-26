---
title: RecurringTaskParameters.IgnoreResourceCalendar
second_title: Aspose.Tasks for .NET API Reference
description: RecurringTaskParameters property. Gets or sets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it
type: docs
weight: 30
url: /net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Gets or sets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it.

```csharp
public bool IgnoreResourceCalendar { get; set; }
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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


