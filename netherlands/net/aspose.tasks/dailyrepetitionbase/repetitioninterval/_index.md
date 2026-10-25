---
title: "DailyRepetitionBase.RepetitionInterval"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "DailyRepetitionBase-eigenschap. Haalt een aantal dagen op of stelt het in, wat het interval in dagen tussen gebeurtenissen vertegenwoordigt"
type: docs
weight: 10
url: /nl/net/aspose.tasks/dailyrepetitionbase/repetitioninterval/
---
## DailyRepetitionBase.RepetitionInterval property

Haalt op of stelt een aantal dagen in dat het interval in dagen tussen gebeurtenissen aangeeft.

```csharp
public int RepetitionInterval { get; set; }
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

* class [DailyRepetitionBase](../)
* namespace [Aspose.Tasks](../../dailyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


