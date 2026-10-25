---
title: "Klasse WeeklyRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeeklyRepetition klasse. Vertegenwoordigt een patroon dat gebaseerd is op weekdagen"
type: docs
weight: 3590
url: /nl/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Stelt een patroon voor dat gebaseerd is op weekdagen.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Initialiseert een nieuw exemplaar van de `WeeklyRepetition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Geeft of stelt een aantal weken in dat het interval in weken tussen de gebeurtenissen vertegenwoordigt. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Haalt op of stelt een type weekdagen in. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


