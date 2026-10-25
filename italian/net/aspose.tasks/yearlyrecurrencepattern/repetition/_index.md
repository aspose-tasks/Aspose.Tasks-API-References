---
title: "YearlyRecurrencePattern.Repetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà YearlyRecurrencePattern. Ottiene o imposta il modello di posizione ricorrente"
type: docs
weight: 20
url: /it/net/aspose.tasks/yearlyrecurrencepattern/repetition/
---
## YearlyRecurrencePattern.Repetition property

Ottiene o imposta il modello di posizione ricorrente.

```csharp
public YearlyRepetitionBase Repetition { get; set; }
```

## Esempi

Mostra come lavorare con i modelli di ricorrenza annuale durante la creazione di attività ricorrenti.

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

project.Save(OutDir + "WorkWithYearlyRecurrencePattern_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [YearlyRepetitionBase](../../yearlyrepetitionbase/)
* class [YearlyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../yearlyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


