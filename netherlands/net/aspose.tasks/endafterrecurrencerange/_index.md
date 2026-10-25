---
title: "Klasse EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.EndAfterRecurrenceRange klasse. Vertegenwoordigt het recursiebereik van een terugkerende taak die beperkt is door het aantal voorkomen."
type: docs
weight: 500
url: /nl/net/aspose.tasks/endafterrecurrencerange/
---
## EndAfterRecurrenceRange class

Stelt het terugkeerbereik van een terugkerende taak voor dat beperkt is door het aantal keren.

```csharp
public class EndAfterRecurrenceRange : RecurrenceRangeBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [EndAfterRecurrenceRange](endafterrecurrencerange/)() | Initialiseert een nieuw exemplaar van de `EndAfterRecurrenceRange`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [OccurrenceNumber](../../aspose.tasks/endafterrecurrencerange/occurrencenumber/) { get; set; } | Haalt op of stelt het aantal voorkomen in dat het recursiebereik van de terugkerende taak beperkt. |
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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


