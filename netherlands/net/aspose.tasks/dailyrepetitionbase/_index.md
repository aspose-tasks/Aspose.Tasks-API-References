---
title: "Klasse DailyRepetitionBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.DailyRepetitionBase klasse. Stelt een basisklasse voor herhalingen in een dagelijks terugkeerpatroon."
type: docs
weight: 410
url: /nl/net/aspose.tasks/dailyrepetitionbase/
---
## DailyRepetitionBase class

Stelt een basisklasse voor herhalingen in een dagelijks terugkeerpatroon voor.

```csharp
public abstract class DailyRepetitionBase
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


