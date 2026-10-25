---
title: "RecurringTaskParameters.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringTaskParameters eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de terugkerende taak moet worden gepland, zelfs als deze niet plaatsvindt wanneer er geen middelen beschikbaar zijn om eraan te werken."
type: docs
weight: 30
url: /nl/net/aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/
---
## RecurringTaskParameters.IgnoreResourceCalendar property

Haalt op of stelt een waarde in die aangeeft of de terugkerende taak gepland moet worden, zelfs als deze niet plaatsvindt wanneer er geen middelen beschikbaar zijn om eraan te werken.

```csharp
public bool IgnoreResourceCalendar { get; set; }
```

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

* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


