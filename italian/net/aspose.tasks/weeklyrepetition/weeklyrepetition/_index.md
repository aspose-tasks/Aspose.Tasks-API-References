---
title: "WeeklyRepetition.WeeklyRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore WeeklyRepetition. Inizializza una nuova istanza della classe WeeklyRepetition"
type: docs
weight: 10
url: /it/net/aspose.tasks/weeklyrepetition/weeklyrepetition/
---
## WeeklyRepetition constructor

Inizializza una nuova istanza della classe [`WeeklyRepetition`](../).

```csharp
public WeeklyRepetition()
```

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

* class [WeeklyRepetition](../)
* namespace [Aspose.Tasks](../../weeklyrepetition/)
* assembly [Aspose.Tasks](../../../)


