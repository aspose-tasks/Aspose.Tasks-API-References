---
title: "Klasse RecurrencePatternBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecurrencePatternBase klasse. Vertegenwoordigt de basisklasse van het terugkeerpatroon"
type: docs
weight: 1700
url: /nl/net/aspose.tasks/recurrencepatternbase/
---
## RecurrencePatternBase class

Stelt de basisklasse van een herhalingspatroon voor.

```csharp
public abstract class RecurrencePatternBase
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Haalt op of stelt het terugkeerbereik in. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


