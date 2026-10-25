---
title: "Classe WeeklyRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WeeklyRepetition. Rappresenta un modello basato sui giorni della settimana"
type: docs
weight: 3590
url: /it/net/aspose.tasks/weeklyrepetition/
---
## WeeklyRepetition class

Rappresenta un modello basato sui giorni della settimana.

```csharp
public class WeeklyRepetition : WeeklyRepetitionBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WeeklyRepetition](weeklyrepetition/)() | Inizializza una nuova istanza della classe `WeeklyRepetition`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/weeklyrepetitionbase/repetitioninterval/) { get; set; } | Ottiene o imposta un numero di settimane che rappresenta l'intervallo in settimane tra le occorrenze. |
| [WeekDays](../../aspose.tasks/weeklyrepetition/weekdays/) { get; set; } | Ottiene o imposta un tipo di giorno della settimana. |

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

* class [WeeklyRepetitionBase](../weeklyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


