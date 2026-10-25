---
title: "Klasse MonthlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.MonthlyRecurrencePattern-klasse. Vertegenwoordigt de set parameters die worden gebruikt om een maandelijks terugkerende taak in een project te maken."
type: docs
weight: 1080
url: /nl/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Stelt de set parameters voor die worden gebruikt om een maandelijks terugkerende taak in een project te maken.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Initialiseert een nieuw exemplaar van de `MonthlyRecurrencePattern`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Haalt op of stelt het terugkeerbereik in. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Haalt het terugkerende herhalingspatroon op of stelt het in. |

## Voorbeelden

Toont hoe te werken met maandelijkse terugkeerpatroonherhalingen bij het maken van terugkerende taken.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


