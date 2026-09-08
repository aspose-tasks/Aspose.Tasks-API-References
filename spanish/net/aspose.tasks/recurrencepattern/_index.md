---
title: "Enumeración RecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.RecurrencePattern. Representa un tipo de patrón de recurrencia de una tarea recurrente"
type: docs
weight: 1690
url: /es/net/aspose.tasks/recurrencepattern/
---
## RecurrencePattern enumeration

Representa un tipo de patrón de recurrencia de una tarea recurrente.

```csharp
[Flags]
public enum RecurrencePattern
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Daily | `1` | Patrón diario. |
| Weekly | `4` | Patrón semanal. |
| Monthly | `8` | Patrón mensual. |
| Yearly | `10` | Patrón anual. |

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


