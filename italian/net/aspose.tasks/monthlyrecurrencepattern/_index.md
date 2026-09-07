---
title: "Classe MonthlyRecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.MonthlyRecurrencePattern. Rappresenta il set di parametri usati per creare un'attività ricorrente mensile in un progetto"
type: docs
weight: 1080
url: /it/net/aspose.tasks/monthlyrecurrencepattern/
---
## MonthlyRecurrencePattern class

Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente mensile in un progetto.

```csharp
public class MonthlyRecurrencePattern : RecurrencePatternBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MonthlyRecurrencePattern](monthlyrecurrencepattern/)() | Inizializza una nuova istanza della classe `MonthlyRecurrencePattern`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Ottiene o imposta l'intervallo di ricorrenza. |
| [Repetition](../../aspose.tasks/monthlyrecurrencepattern/repetition/) { get; set; } | Ottiene o imposta il modello di ripetizione ricorrente. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


