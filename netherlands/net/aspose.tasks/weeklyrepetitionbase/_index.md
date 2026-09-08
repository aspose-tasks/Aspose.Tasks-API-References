---
title: "Klasse WeeklyRepetitionBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WeeklyRepetitionBase‑klasse. Vertegenwoordigt een basisklasse voor herhalingen in een wekelijks recursiepatroon"
type: docs
weight: 3600
url: /nl/net/aspose.tasks/weeklyrepetitionbase/
---
## WeeklyRepetitionBase class

Stelt een basisklasse voor voor herhalingen in een wekelijks terugkeerpatroon.

```csharp
public abstract class WeeklyRepetitionBase
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Geeft of stelt een aantal weken in dat het interval in weken tussen de gebeurtenissen vertegenwoordigt. |

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


