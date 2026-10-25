---
title: "Enum WeekdayType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.WeekdayType. Rappresenta un giorno della settimana di un progetto nell'istanza della classe RecurringTaskInfo."
type: docs
weight: 3570
url: /it/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Rappresenta un giorno della settimana di un progetto nell'istanza della classe [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Indica il tipo di giorno della settimana None. |
| Sunday | `1` | Indica il tipo di giorno della settimana Sunday. |
| Monday | `2` | Indica il tipo di giorno della settimana Monday. |
| Tuesday | `4` | Indica il tipo di giorno della settimana Tuesday. |
| Wednesday | `8` | Indica il tipo di giorno della settimana Wednesday. |
| Thursday | `10` | Indica il tipo di giorno della settimana Thursday. |
| Friday | `20` | Indica il tipo di giorno della settimana Friday. |
| Saturday | `40` | Indica il tipo di giorno della settimana Saturday. |

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


