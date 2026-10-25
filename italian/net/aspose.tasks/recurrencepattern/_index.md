---
title: "Enum RecurrencePattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.RecurrencePattern. Rappresenta un tipo di modello di ricorrenza di un'attività ricorrente."
type: docs
weight: 1690
url: /it/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Rappresenta un tipo di modello di ricorrenza di un'attività ricorrente.

```csharp
[Flags]
public enum RecurrencePattern
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Daily | `1` | Modello giornaliero. |
| Weekly | `4` | Modello settimanale. |
| Monthly | `8` | Modello mensile. |
| Yearly | `10` | Modello annuale. |

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


