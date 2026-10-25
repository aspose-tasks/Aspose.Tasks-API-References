---
title: "Klasse ByYearDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ByYearDayRepetition klasse. Vertegenwoordigt een patroon dat gebaseerd is op de absolute positie van een dag in een maand"
type: docs
weight: 190
url: /nl/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Stelt een patroon voor dat gebaseerd is op de absolute positie van een dag in een maand.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Initialiseert een nieuwe instantie van de `ByYearDayRepetition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Haalt een positie van een dag in een maand op of stelt deze in waarop de taak moet terugkeren. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Haalt een maand op of stelt een maand in waarop de taak moet terugkeren. |

## Voorbeelden

Toont hoe te werken met jaar-dag herhalingen bij het maken van nieuwe terugkerende taken.

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

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


