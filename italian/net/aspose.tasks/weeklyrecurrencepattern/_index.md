---
title: "Classe WeeklyRecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WeeklyRecurrencePattern. Rappresenta l'insieme di parametri utilizzati per creare un'attività ricorrente settimanale in un progetto."
type: docs
weight: 3580
url: /it/net/aspose.tasks/weeklyrecurrencepattern/
---
## WeeklyRecurrencePattern class

Rappresenta l'insieme dei parametri utilizzati per creare un'attività ricorrente settimanale in un progetto.

```csharp
public class WeeklyRecurrencePattern : RecurrencePatternBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WeeklyRecurrencePattern](weeklyrecurrencepattern/)() | Inizializza una nuova istanza della classe `WeeklyRecurrencePattern`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Ottiene o imposta l'intervallo di ricorrenza. |
| [Repetition](../../aspose.tasks/weeklyrecurrencepattern/repetition/) { get; set; } | Ottiene o imposta il modello di ripetizione ricorrente. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


