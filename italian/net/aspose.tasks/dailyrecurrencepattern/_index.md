---
title: "Classe DailyRecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.DailyRecurrencePattern. Rappresenta l'insieme dei parametri utilizzati per creare un'attività ricorrente giornaliera in un progetto"
type: docs
weight: 400
url: /it/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente giornaliera in un progetto.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Inizializza una nuova istanza della classe `DailyRecurrencePattern`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Ottiene o imposta l'intervallo di ricorrenza. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Ottiene o imposta il modello di ripetizioni nel modello di ricorrenza giornaliera. |

## Esempi

Mostra come lavorare con le ripetizioni del modello di ripetizione giornaliera durante la creazione di attività ricorrenti.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// continua a lavorare sul progetto...
// ...
```

### Vedi anche

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


