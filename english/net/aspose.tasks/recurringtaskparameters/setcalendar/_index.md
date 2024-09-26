---
title: RecurringTaskParameters.SetCalendar
second_title: Aspose.Tasks for .NET API Reference
description: RecurringTaskParameters method. Set a calendar for recurring task. The calendar is selected from project calendar collection
type: docs
weight: 60
url: /net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Set a calendar for recurring task. The calendar is selected from project calendar collection.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| project | Project | The project with calendar collection. |
| calendarName | String | The name of calendar. |

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

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


