---
title: "Class ByMonthDayRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ByMonthDayRepetition. Rappresenta un modello basato sulla posizione assoluta di un giorno in un mese"
type: docs
weight: 170
url: /it/net/aspose.tasks/bymonthdayrepetition/
---
## ByMonthDayRepetition class

Rappresenta un modello basato sulla posizione assoluta di un giorno in un mese.

```csharp
public class ByMonthDayRepetition : MonthlyRepetitionBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ByMonthDayRepetition](bymonthdayrepetition/)() | Inizializza una nuova istanza della classe `ByMonthDayRepetition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DayPosition](../../aspose.tasks/bymonthdayrepetition/dayposition/) { get; set; } | Ottiene o imposta la posizione di un giorno in un mese in cui l'attività deve ripetersi. |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Ottiene o imposta il numero di mesi che rappresenta l'intervallo in mesi tra le occorrenze. |

## Esempi

Mostra come lavorare con le ripetizioni giorno del mese durante la creazione di nuove attività ricorrenti.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new MonthlyRecurrencePattern
                                                 {
                                                     Repetition = new ByMonthDayRepetition { DayPosition = 1, RepetitionInterval = 2 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 9, 30, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Months_EndByRecurrenceRange_Test_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [MonthlyRepetitionBase](../monthlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


