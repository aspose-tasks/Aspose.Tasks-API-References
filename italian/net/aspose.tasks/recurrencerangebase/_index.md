---
title: "Classe RecurrenceRangeBase"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RecurrenceRangeBase. Rappresenta l'intervallo di ricorrenza di un'attività ricorrente."
type: docs
weight: 1710
url: /it/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

Rappresenta l'intervallo di ricorrenza di un'attività ricorrente.

```csharp
public abstract class RecurrenceRangeBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Ottiene o imposta la data di inizio dell'intervallo di ricorrenza dell'attività ricorrente. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


