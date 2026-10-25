---
title: "Klasse DailyWorkRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DailyWorkRepetition klasse. Vertegenwoordigt een klasse voor herhalingen in een dagelijks terugkeerpatroon op basis van werkdagen"
type: docs
weight: 420
url: /nl/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Stelt een klasse voor herhalingen in een dagelijks terugkeerpatroon gebaseerd op werkdagen.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Initialiseert een nieuw exemplaar van de `DailyWorkRepetition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Haalt op of stelt een aantal dagen in dat het interval in dagen tussen gebeurtenissen aangeeft. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


