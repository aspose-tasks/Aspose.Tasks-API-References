---
title: "Klasse RecurringTaskParameters"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecurringTaskParameters klasse. Vertegenwoordigt de set parameters die worden gebruikt om een terugkerende taak in een project te maken"
type: docs
weight: 1730
url: /nl/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Stelt de set parameters voor die worden gebruikt om een terugkerende taak in een project te maken.

```csharp
public class RecurringTaskParameters
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Initialiseert een nieuw exemplaar van de `RecurringTaskParameters` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Haalt op of stelt de duur in voor één voorkomen van de terugkerende taak. Het exemplaar van de [`Duration`](./duration/) klasse. |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de terugkerende taak gepland moet worden, zelfs als deze niet plaatsvindt wanneer er geen middelen beschikbaar zijn om eraan te werken. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Haalt op of stelt het terugkeerpatroon van de terugkerende taak in. Kan een van de waarden van de [`RecurrencePattern`](./recurrencepattern/) enumeratie zijn. |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Haalt op of stelt de naam van de terugkerende taak in. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Stel een agenda in voor de terugkerende taak. De agenda wordt geselecteerd uit de projectagendacollectie. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


