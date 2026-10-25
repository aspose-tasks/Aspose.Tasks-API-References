---
title: "DailyWorkRepetition.DailyWorkRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di DailyWorkRepetition. Inizializza una nuova istanza della classe DailyWorkRepetition"
type: docs
weight: 10
url: /it/net/aspose.tasks/dailyworkrepetition/dailyworkrepetition/
---
## DailyWorkRepetition constructor

Inizializza una nuova istanza della classe [`DailyWorkRepetition`](../).

```csharp
public DailyWorkRepetition()
```

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

* class [DailyWorkRepetition](../)
* namespace [Aspose.Tasks](../../dailyworkrepetition/)
* assembly [Aspose.Tasks](../../../)


