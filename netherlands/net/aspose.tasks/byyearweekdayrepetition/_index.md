---
title: "Klasse ByYearWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ByYearWeekDayRepetition klasse. Vertegenwoordigt een patroon dat gebaseerd is op de positie van een weekdag in een maand"
type: docs
weight: 200
url: /nl/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Stelt een patroon voor dat gebaseerd is op de positie van een weekdag in een maand.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Initialiseert een nieuwe instantie van de `ByYearWeekDayRepetition` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Haalt een maand op of stelt een maand in waarop de taak moet terugkeren. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Haalt een positie van de dag in een week van een maand op of stelt een positie in waarop de taak moet terugkeren. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Haalt op of stelt een type weekdag in waarop de taak moet terugkeren. |

## Voorbeelden

Toont hoe te werken met herhalingen van weekdagen per jaar bij het maken van nieuwe terugkerende taken.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearWeekDayRepetition
                                                                      {
                                                                          Month = Month.July, WeekDay = DayOfWeek.Sunday, Position = OrdinalNumber.First
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 31, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearWeekDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


