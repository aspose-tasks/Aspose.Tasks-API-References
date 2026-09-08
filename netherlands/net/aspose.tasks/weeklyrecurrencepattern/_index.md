---
title: "Klasse WeeklyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeeklyRecurrencePattern klasse. Vertegenwoordigt de set parameters die worden gebruikt om een wekelijks terugkerende taak in een project te maken"
type: docs
weight: 3580
url: /nl/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Stelt de set parameters voor die worden gebruikt om een wekelijks terugkerende taak in een project te maken.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Initialiseert een nieuw exemplaar van de `WeeklyRecurrencePattern`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Haalt op of stelt het terugkeerbereik in. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Haalt het terugkerende herhalingspatroon op of stelt het in. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


