---
title: "Klasse YearlyRecurrencePattern"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.YearlyRecurrencePattern class. Vertegenwoordigt de set parameters die worden gebruikt om een jaarlijks terugkerende taak in een project te maken."
type: docs
weight: 3690
url: /nl/net/aspose.tasks/yearlyrecurrencepattern/
---
## YearlyRecurrencePattern class

Stelt de set parameters voor die worden gebruikt om een jaarlijks terugkerende taak in een project te maken.

```csharp
public class YearlyRecurrencePattern : RecurrencePatternBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [YearlyRecurrencePattern](yearlyrecurrencepattern/)() | Initialiseert een nieuw exemplaar van de `YearlyRecurrencePattern` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Haalt op of stelt het terugkeerbereik in. |
| [Repetition](../../aspose.tasks/yearlyrecurrencepattern/repetition/) { get; set; } | Haalt op of stelt het terugkerende positiepatroon in. |

## Voorbeelden

Toont hoe te werken met year year terugkeerpatronen bij het maken van terugkerende taken.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


