---
title: "RecurringTaskParameters.Duration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà RecurringTaskParameters. Ottiene o imposta la durata per una singola occorrenza dell'attività ricorrente. L'istanza della classe Duration"
type: docs
weight: 20
url: /it/net/aspose.tasks/recurringtaskparameters/duration/
---
## RecurringTaskParameters.Duration property

Ottiene o imposta la durata per una singola occorrenza dell'attività ricorrente. L'istanza della classe `Duration`.

```csharp
public Duration Duration { get; set; }
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

* struct [Duration](../../duration/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


