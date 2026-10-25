---
title: "Classe ByYearDayRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ByYearDayRepetition. Rappresenta un modello basato sulla posizione assoluta di un giorno in un mese"
type: docs
weight: 190
url: /it/net/aspose.tasks/byyeardayrepetition/
---
## ByYearDayRepetition class

Rappresenta un modello basato sulla posizione assoluta di un giorno in un mese.

```csharp
public class ByYearDayRepetition : YearlyRepetitionBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ByYearDayRepetition](byyeardayrepetition/)() | Inizializza una nuova istanza della classe `ByYearDayRepetition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DayPosition](../../aspose.tasks/byyeardayrepetition/dayposition/) { get; set; } | Ottiene o imposta una posizione del giorno in un mese in cui l'attività deve essere ricorrente. |
| [Month](../../aspose.tasks/byyeardayrepetition/month/) { get; set; } | Ottiene o imposta il mese in cui l'attività deve ricorrere. |

## Esempi

Mostra come lavorare con le ripetizioni giornaliere annuali durante la creazione di nuove attività ricorrenti.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [YearlyRepetitionBase](../yearlyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


