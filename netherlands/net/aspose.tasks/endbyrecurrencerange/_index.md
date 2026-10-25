---
title: "Klasse EndByRecurrenceRange"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.EndByRecurrenceRange klasse. Vertegenwoordigt het recursiebereik van een terugkerende taak die beperkt is door de einddag."
type: docs
weight: 510
url: /nl/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Stelt het terugkeerbereik van een terugkerende taak voor dat beperkt is door de einddag.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Initialiseert een nieuw exemplaar van de `EndByRecurrenceRange` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Haalt op of stelt de datum in die het recursiebereik van de terugkerende taak beperkt. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Haalt op of stelt de startdatum van het recursiebereik van de terugkerende taak in. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


