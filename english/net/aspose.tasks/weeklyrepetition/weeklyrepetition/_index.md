---
title: WeeklyRepetition.WeeklyRepetition
second_title: Aspose.Tasks for .NET API Reference
description: WeeklyRepetition constructor. Initializes a new instance of the WeeklyRepetition class
type: docs
weight: 10
url: /net/aspose.tasks/weeklyrepetition/weeklyrepetition/
---
## WeeklyRepetition constructor

Initializes a new instance of the [`WeeklyRepetition`](../) class.

```csharp
public WeeklyRepetition()
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

* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


