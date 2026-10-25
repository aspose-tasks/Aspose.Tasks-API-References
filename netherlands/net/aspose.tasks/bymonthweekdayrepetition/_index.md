---
title: "Klasse ByMonthWeekDayRepetition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ByMonthWeekDayRepetition‑klasse. Vertegenwoordigt een patroon dat gebaseerd is op de positie van een weekdag in een maand."
type: docs
weight: 180
url: /nl/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Stelt een patroon voor dat gebaseerd is op de positie van een weekdag in een maand.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Initialiseert een nieuw exemplaar van de `ByMonthWeekDayRepetition`‑klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Haalt op of stelt een positie van een weekdag in een maand in waarop de taak moet terugkeren. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Haalt een aantal maanden op of stelt dit in dat het interval in maanden tussen de gebeurtenissen vertegenwoordigt. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Haalt op of stelt een type weekdag in waarop de taak moet terugkeren. |

## Voorbeelden

Toont hoe te werken met maand‑weekdag‑herhalingen bij het maken van nieuwe terugkerende taken.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthWeekDayRepetition
                                                                      {
                                                                          Position = OrdinalNumber.First,
                                                                          WeekDay = DayOfWeek.Sunday,
                                                                          RepetitionInterval = 2
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 2, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);
project.Save(OutDir + "CanAddRecurringTask_Months_WeekDay_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


