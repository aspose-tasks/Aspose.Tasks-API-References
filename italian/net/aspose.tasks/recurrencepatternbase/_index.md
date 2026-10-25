---
title: "Classe RecurrencePatternBase"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RecurrencePatternBase. Rappresenta la classe base del modello di ricorrenza"
type: docs
weight: 1700
url: /it/net/aspose.tasks/recurrencepatternbase/
---
## RecurrencePatternBase class

Rappresenta la classe base del modello di ricorrenza.

```csharp
public abstract class RecurrencePatternBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Ottiene o imposta l'intervallo di ricorrenza. |

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


