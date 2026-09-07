---
title: "MonthlyRepetitionBase.RepetitionInterval"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MonthlyRepetitionBase. Ottiene o imposta un numero di mesi che rappresenta l'intervallo in mesi tra le occorrenze."
type: docs
weight: 10
url: /it/net/aspose.tasks/monthlyrepetitionbase/repetitioninterval/
---
## MonthlyRepetitionBase.RepetitionInterval property

Ottiene o imposta il numero di mesi che rappresenta l'intervallo in mesi tra le occorrenze.

```csharp
public int RepetitionInterval { get; set; }
```

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

* class [MonthlyRepetitionBase](../)
* namespace [Aspose.Tasks](../../monthlyrepetitionbase/)
* assembly [Aspose.Tasks](../../../)


