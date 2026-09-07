---
title: "WeeklyRecurrencePattern.Repetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà WeeklyRecurrencePattern. Ottiene o imposta il modello di ripetizione ricorrente"
type: docs
weight: 20
url: /it/net/aspose.tasks/weeklyrecurrencepattern/repetition/
---
## WeeklyRecurrencePattern.Repetition property

Ottiene o imposta il modello di ripetizione ricorrente.

```csharp
public WeeklyRepetitionBase Repetition { get; set; }
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

* class [WeeklyRepetitionBase](../../weeklyrepetitionbase/)
* class [WeeklyRecurrencePattern](../)
* namespace [Aspose.Tasks](../../weeklyrecurrencepattern/)
* assembly [Aspose.Tasks](../../../)


