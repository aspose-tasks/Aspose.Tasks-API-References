---
title: "RecurringTaskParameters.RecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà RecurringTaskParameters. Ottiene o imposta il modello di ricorrenza dell'attività ricorrente. Può essere uno dei valori dell'enumerazione RecurrencePattern"
type: docs
weight: 40
url: /it/net/aspose.tasks/recurringtaskparameters/recurrencepattern/
---
## RecurringTaskParameters.RecurrencePattern property

Ottiene o imposta il modello di ricorrenza dell'attività ricorrente. Può essere uno dei valori dell'enumerazione `RecurrencePattern`.

```csharp
public RecurrencePatternBase RecurrencePattern { get; set; }
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

* class [RecurrencePatternBase](../../recurrencepatternbase/)
* class [RecurringTaskParameters](../)
* namespace [Aspose.Tasks](../../recurringtaskparameters/)
* assembly [Aspose.Tasks](../../../)


