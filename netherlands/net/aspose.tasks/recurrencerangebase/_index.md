---
title: "Klasse RecurrenceRangeBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.RecurrenceRangeBase klasse. Vertegenwoordigt het terugkeerbereik van een terugkerende taak."
type: docs
weight: 1710
url: /nl/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

Stelt het herhalingsbereik van een terugkerende taak voor.

```csharp
public abstract class RecurrenceRangeBase
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Haalt op of stelt de startdatum van het recursiebereik van de terugkerende taak in. |

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


