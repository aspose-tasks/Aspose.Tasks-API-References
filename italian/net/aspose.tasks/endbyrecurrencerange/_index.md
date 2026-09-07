---
title: "Classe EndByRecurrenceRange"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.EndByRecurrenceRange. Rappresenta l'intervallo di ricorrenza di un'attività ricorrente limitato dal giorno di fine"
type: docs
weight: 510
url: /it/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Rappresenta l'intervallo di ricorrenza di un'attività ricorrente limitato dal giorno di fine.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Inizializza una nuova istanza della classe `EndByRecurrenceRange`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Ottiene o imposta la data che limita l'intervallo di ricorrenza dell'attività ricorrente. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Ottiene o imposta la data di inizio dell'intervallo di ricorrenza dell'attività ricorrente. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


