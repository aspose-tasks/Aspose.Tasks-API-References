---
title: "ByMonthWeekDayRepetition.Position"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ByMonthWeekDayRepetition. Ottiene o imposta una posizione del giorno della settimana in un mese in cui l'attività deve ripetersi"
type: docs
weight: 20
url: /it/net/aspose.tasks/bymonthweekdayrepetition/position/
---
## ByMonthWeekDayRepetition.Position property

Ottiene o imposta una posizione del giorno della settimana in un mese in cui l'attività deve ripetersi.

```csharp
public OrdinalNumber Position { get; set; }
```

## Esempi

Mostra come lavorare con le ripetizioni di giorni della settimana mensili creando nuove attività ricorrenti.

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

### Vedi anche

* enum [OrdinalNumber](../../ordinalnumber/)
* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


