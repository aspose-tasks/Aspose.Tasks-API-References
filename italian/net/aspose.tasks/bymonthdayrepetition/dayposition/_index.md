---
title: "ByMonthDayRepetition.DayPosition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "ByMonthDayRepetition proprietà. Ottiene o imposta una posizione di un giorno in un mese in cui l'attività deve ripetersi"
type: docs
weight: 20
url: /it/net/aspose.tasks/bymonthdayrepetition/dayposition/
---
## ByMonthDayRepetition.DayPosition property

Ottiene o imposta la posizione di un giorno in un mese in cui l'attività deve ripetersi.

```csharp
public int DayPosition { get; set; }
```

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

* class [ByMonthDayRepetition](../)
* namespace [Aspose.Tasks](../../bymonthdayrepetition/)
* assembly [Aspose.Tasks](../../../)


