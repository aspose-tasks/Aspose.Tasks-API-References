---
title: "Enumeración WeekdayType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.WeekdayType enum. Representa un día de la semana de un proyecto en la instancia de la clase RecurringTaskInfo"
type: docs
weight: 3570
url: /es/net/aspose.tasks/weekdaytype/
---
## WeekdayType enumeration

Representa un día de la semana de un proyecto en la instancia de la clase [`RecurringTaskInfo`](../recurringtaskinfo/).

```csharp
[Flags]
public enum WeekdayType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Indica el tipo de día de la semana None. |
| Sunday | `1` | Indica el tipo de día de la semana Sunday. |
| Monday | `2` | Indica el tipo de día de la semana Monday. |
| Tuesday | `4` | Indica el tipo de día de la semana Tuesday. |
| Wednesday | `8` | Indica el tipo de día de la semana Wednesday. |
| Thursday | `10` | Indica el tipo de día de la semana Thursday. |
| Friday | `20` | Indica el tipo de día de la semana Friday. |
| Saturday | `40` | Indica el tipo de día de la semana Saturday. |

## Ejemplos

Muestra cómo crear una tarea recurrente.

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

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


