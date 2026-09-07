---
title: "Classe MonthlyRepetitionBase"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.MonthlyRepetitionBase. Rappresenta un modello di base per la posizione giornaliera mensile."
type: docs
weight: 1090
url: /it/net/aspose.tasks/monthlyrepetitionbase/
---
## MonthlyRepetitionBase class

Rappresenta un modello di base per la posizione del giorno mensile.

```csharp
public abstract class MonthlyRepetitionBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/monthlyrepetitionbase/repetitioninterval/) { get; set; } | Ottiene o imposta il numero di mesi che rappresenta l'intervallo in mesi tra le occorrenze. |

## Esempi

Mostra come lavorare con le ripetizioni del modello di ricorrenza mensile durante la creazione di attività ricorrenti.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


