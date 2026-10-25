---
title: "RecurrenceRangeBase.Start"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurrenceRangeBase‑eigenschap. Haalt de startdatum op of stelt deze in van het herhalingsbereik van de terugkerende taak"
type: docs
weight: 10
url: /nl/net/aspose.tasks/recurrencerangebase/start/
---
## RecurrenceRangeBase.Start property

Haalt op of stelt de startdatum van het recursiebereik van de terugkerende taak in.

```csharp
public DateTime Start { get; set; }
```

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

* class [RecurrenceRangeBase](../)
* namespace [Aspose.Tasks](../../recurrencerangebase/)
* assembly [Aspose.Tasks](../../../)


