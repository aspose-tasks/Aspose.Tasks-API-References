---
title: "Classe ByYearWeekDayRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ByYearWeekDayRepetition. Rappresenta un modello basato sulla posizione di un giorno della settimana in un mese"
type: docs
weight: 200
url: /it/net/aspose.tasks/byyearweekdayrepetition/
---
## ByYearWeekDayRepetition class

Rappresenta un modello basato sulla posizione di un giorno della settimana in un mese.

```csharp
public class ByYearWeekDayRepetition : YearlyRepetitionBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ByYearWeekDayRepetition](byyearweekdayrepetition/)() | Inizializza una nuova istanza della classe `ByYearWeekDayRepetition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Month](../../aspose.tasks/byyearweekdayrepetition/month/) { get; set; } | Ottiene o imposta il mese in cui l'attività deve ricorrere. |
| [Position](../../aspose.tasks/byyearweekdayrepetition/position/) { get; set; } | Ottiene o imposta la posizione del giorno in una settimana di un mese in cui l'attività deve ricorrere. |
| [WeekDay](../../aspose.tasks/byyearweekdayrepetition/weekday/) { get; set; } | Ottiene o imposta un tipo di giorno della settimana in cui l'attività deve essere ricorrente. |

## Esempi

Mostra come gestire le ripetizioni dei giorni della settimana su base annua durante la creazione di nuove attività ricorrenti.

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

### Vedi anche

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


