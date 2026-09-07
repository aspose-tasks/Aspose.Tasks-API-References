---
title: "ByYearDayRepetition.DayPosition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ByYearDayRepetition. Ottiene o imposta una posizione del giorno in un mese in cui l'attività deve essere ricorrente"
type: docs
weight: 20
url: /it/net/aspose.tasks/byyeardayrepetition/dayposition/
---
## ByYearDayRepetition.DayPosition property

Ottiene o imposta una posizione del giorno in un mese in cui l'attività deve essere ricorrente.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByYearDayRepetition](../)
* namespace [Aspose.Tasks](../../byyeardayrepetition/)
* assembly [Aspose.Tasks](../../../)


