---
title: "RecurrencePatternBase.RecurrenceRange"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurrencePatternBase property. Haalt of stelt het herhalingsbereik in"
type: docs
weight: 10
url: /nl/net/aspose.tasks/recurrencepatternbase/recurrencerange/
---
## RecurrencePatternBase.RecurrenceRange property

Haalt op of stelt het terugkeerbereik in.

```csharp
public RecurrenceRangeBase RecurrenceRange { get; set; }
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

* class [RecurrenceRangeBase](../../recurrencerangebase/)
* class [RecurrencePatternBase](../)
* namespace [Aspose.Tasks](../../recurrencepatternbase/)
* assembly [Aspose.Tasks](../../../)


