---
title: "Classe RecurringTaskParameters"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.RecurringTaskParameters. Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente in un progetto"
type: docs
weight: 1730
url: /it/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente in un progetto.

```csharp
public class RecurringTaskParameters
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Inizializza una nuova istanza della classe `RecurringTaskParameters`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Ottiene o imposta la durata per una singola occorrenza dell'attività ricorrente. L'istanza della classe [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Ottiene o imposta un valore che indica se pianificare l'attività ricorrente anche se non si verifica quando non ci sono risorse disponibili per lavorarci. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Ottiene o imposta il modello di ricorrenza dell'attività ricorrente. Può essere uno dei valori dell'enumerazione [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Ottiene o imposta il nome dell'attività ricorrente. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Imposta un calendario per l'attività ricorrente. Il calendario è selezionato dalla raccolta di calendari del progetto. |

## Esempi

Mostra come creare un task ricorrente.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "Recurring task",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new WeeklyRecurrencePattern
                                                 {
                                                     Repetition = new WeeklyRepetition
                                                                      {
                                                                          RepetitionInterval = 2,
                                                                          WeekDays = WeekdayType.Sunday | WeekdayType.Monday | WeekdayType.Friday
                                                                      },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2018, 7, 20, 17, 0, 0)
                                                                           }
                                                 },
                         IgnoreResourceCalendar = false
                     };

parameters.SetCalendar(project, "Standard");

project.RootTask.Children.Add(parameters);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


