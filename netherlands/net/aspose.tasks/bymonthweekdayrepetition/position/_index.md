---
title: "ByMonthWeekDayRepetition.Position"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByMonthWeekDayRepetition eigenschap. Haalt een positie van een weekdag in een maand op of stelt deze in waarop de taak moet terugkeren"
type: docs
weight: 20
url: /nl/net/aspose.tasks/bymonthweekdayrepetition/position/
---
## ByMonthWeekDayRepetition.Position property

Haalt op of stelt een positie van een weekdag in een maand in waarop de taak moet terugkeren.

```csharp
public OrdinalNumber Position { get; set; }
```

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

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


