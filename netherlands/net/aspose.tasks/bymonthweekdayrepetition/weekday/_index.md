---
title: "ByMonthWeekDayRepetition.WeekDay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ByMonthWeekDayRepetition eigenschap. Haalt op of stelt een type weekdag in waarop de taak moet terugkeren"
type: docs
weight: 30
url: /nl/net/aspose.tasks/bymonthweekdayrepetition/weekday/
---
## ByMonthWeekDayRepetition.WeekDay property

Haalt op of stelt een type weekdag in waarop de taak moet terugkeren.

```csharp
public DayOfWeek WeekDay { get; set; }
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

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


