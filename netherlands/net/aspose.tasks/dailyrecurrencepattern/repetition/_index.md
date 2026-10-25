---
title: "DailyRecurrencePattern.Repetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DailyRecurrencePattern-eigenschap. Haalt het patroon van herhalingen in het dagelijkse recursiepatroon op of stelt dit in"
type: docs
weight: 20
url: /nl/net/aspose.tasks/dailyrecurrencepattern/repetition/
---
## DailyRecurrencePattern.Repetition property

Haalt op of stelt het patroon van herhalingen in het dagelijkse terugkeerpatroon in.

```csharp
public DailyRepetitionBase Repetition { get; set; }
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

* class [DailyRepetitionBase](../../dailyrepetitionbase/)
* class [DailyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../dailyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


