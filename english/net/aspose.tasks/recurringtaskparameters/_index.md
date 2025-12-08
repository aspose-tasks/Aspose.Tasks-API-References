---
title: Class RecurringTaskParameters
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RecurringTaskParameters class. Represents the set of parameters are used to create a recurring task in a project
type: docs
weight: 1700
url: /net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Represents the set of parameters are used to create a recurring task in a project.

```csharp
public class RecurringTaskParameters
```

## Constructors

| Name | Description |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Initializes a new instance of the `RecurringTaskParameters` class. |

## Properties

| Name | Description |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Gets or sets the duration for one occurrence of the recurring task. The instance of [`Duration`](./duration/) class. |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Gets or sets a value indicating whether to schedule the recurring task even if it does not happen when any resources are available to work on it. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Gets or sets the recurrence pattern of the recurring task. Can be one of the values of [`RecurrencePattern`](./recurrencepattern/) enumeration. |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Gets or sets the name of the recurring task. |

## Methods

| Name | Description |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Set a calendar for recurring task. The calendar is selected from project calendar collection. |

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


