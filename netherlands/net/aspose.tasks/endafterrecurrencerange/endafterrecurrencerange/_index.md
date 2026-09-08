---
title: "EndAfterRecurrenceRange.EndAfterRecurrenceRange"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "EndAfterRecurrenceRange constructor. Initialiseert een nieuw exemplaar van de EndAfterRecurrenceRange klasse."
type: docs
weight: 10
url: /nl/net/aspose.tasks/endafterrecurrencerange/endafterrecurrencerange/
---
## EndAfterRecurrenceRange constructor

Initialiseert een nieuw exemplaar van de [`EndAfterRecurrenceRange`](../) klasse.

```csharp
public EndAfterRecurrenceRange()
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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


