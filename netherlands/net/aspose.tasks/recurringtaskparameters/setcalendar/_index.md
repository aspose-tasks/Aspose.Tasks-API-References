---
title: "RecurringTaskParameters.SetCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringTaskParameters methode. Stel een agenda in voor de terugkerende taak. De agenda wordt geselecteerd uit de projectagenda‑collectie."
type: docs
weight: 60
url: /nl/net/aspose.tasks/recurringtaskparameters/setcalendar/
---
## RecurringTaskParameters.SetCalendar method

Stel een agenda in voor de terugkerende taak. De agenda wordt geselecteerd uit de projectagendacollectie.

```csharp
public void SetCalendar(Project project, string calendarName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| project | Project | Het project met agenda‑collectie. |
| calendarName | String | De naam van de agenda. |

## Voorbeelden

Toont hoe een terugkerende taak te maken.

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

### Zie ook

* class [Project](../../project/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


