---
title: "Clase EndByRecurrenceRange"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.EndByRecurrenceRange. Representa el rango de recurrencia de una tarea recurrente que está limitado por el día de finalización."
type: docs
weight: 510
url: /es/net/aspose.tasks/endbyrecurrencerange/
---
## EndByRecurrenceRange class

Representa el rango de recurrencia de una tarea recurrente que está limitado por el día de finalización.

```csharp
public class EndByRecurrenceRange : RecurrenceRangeBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [EndByRecurrenceRange](endbyrecurrencerange/)() | Inicializa una nueva instancia de la clase `EndByRecurrenceRange`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Finish](../../aspose.tasks/endbyrecurrencerange/finish/) { get; set; } | Obtiene o establece la fecha que limita el rango de recurrencia de la tarea recurrente. |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Obtiene o establece la fecha de inicio del rango de recurrencia de la tarea recurrente. |

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

* class [RecurrenceRangeBase](../recurrencerangebase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


