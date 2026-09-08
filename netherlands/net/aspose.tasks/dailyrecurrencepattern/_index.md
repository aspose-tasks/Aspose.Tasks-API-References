---
title: "Klasse DailyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DailyRecurrencePattern klasse. Vertegenwoordigt de set parameters die worden gebruikt om een dagelijks terugkerende taak in een project te maken."
type: docs
weight: 400
url: /nl/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Stelt de set parameters voor die worden gebruikt om een dagelijkse terugkerende taak in een project te maken.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Initialiseert een nieuw exemplaar van de `DailyRecurrencePattern` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Haalt op of stelt het terugkeerbereik in. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Haalt op of stelt het patroon van herhalingen in het dagelijkse terugkeerpatroon in. |

## Voorbeelden

Toont hoe te werken met herhalingen van het dagelijkse werkherhalingspatroon bij het maken van terugkerende taken.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// werk verder met het project...
// ...
```

### Zie ook

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


