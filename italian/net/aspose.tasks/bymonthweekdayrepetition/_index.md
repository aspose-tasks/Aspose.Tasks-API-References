---
title: "Classe ByMonthWeekDayRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ByMonthWeekDayRepetition. Rappresenta un modello basato sulla posizione del giorno della settimana in un mese"
type: docs
weight: 180
url: /it/net/aspose.tasks/bymonthweekdayrepetition/
---
## ByMonthWeekDayRepetition class

Rappresenta un modello basato sulla posizione del giorno della settimana in un mese.

```csharp
public class ByMonthWeekDayRepetition : MonthlyRepetitionBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ByMonthWeekDayRepetition](bymonthweekdayrepetition/)() | Inizializza una nuova istanza della classe `ByMonthWeekDayRepetition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Position](../../aspose.tasks/bymonthweekdayrepetition/position/) { get; set; } | Ottiene o imposta una posizione del giorno della settimana in un mese in cui l'attività deve ripetersi. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Ottiene o imposta il numero di mesi che rappresenta l'intervallo in mesi tra le occorrenze. |
| [WeekDay](../../aspose.tasks/bymonthweekdayrepetition/weekday/) { get; set; } | Ottiene o imposta un tipo di giorno della settimana in cui l'attività deve ripetersi. |

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

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


