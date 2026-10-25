---
title: "ByMonthWeekDayRepetition.ByMonthWeekDayRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore ByMonthWeekDayRepetition. Inizializza una nuova istanza della classe ByMonthWeekDayRepetition"
type: docs
weight: 10
url: /it/net/aspose.tasks/bymonthweekdayrepetition/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition constructor

Inizializza una nuova istanza della classe [`ByMonthWeekDayRepetition`](../).

```csharp
public ByMonthWeekDayRepetition()
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

* class [ByMonthWeekDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthweekdayrepetition/)
* assembly [Aspose.Tasks](../../../)


