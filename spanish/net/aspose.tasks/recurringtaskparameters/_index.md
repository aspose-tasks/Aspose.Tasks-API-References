---
title: "Clase RecurringTaskParameters"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RecurringTaskParameters. Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente en un proyecto"
type: docs
weight: 1730
url: /es/net/aspose.tasks/recurringtaskparameters/
---
## RecurringTaskParameters class

Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente en un proyecto.

```csharp
public class RecurringTaskParameters
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RecurringTaskParameters](recurringtaskparameters/)() | Inicializa una nueva instancia de la clase `RecurringTaskParameters`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Duration](../../aspose.tasks/recurringtaskparameters/duration/) { get; set; } | Obtiene o establece la duración de una ocurrencia de la tarea recurrente. La instancia de la clase [`Duration`](./duration/). |
| [IgnoreResourceCalendar](../../aspose.tasks/recurringtaskparameters/ignoreresourcecalendar/) { get; set; } | Obtiene o establece un valor que indica si programar la tarea recurrente incluso cuando no hay recursos disponibles para trabajar en ella. |
| [RecurrencePattern](../../aspose.tasks/recurringtaskparameters/recurrencepattern/) { get; set; } | Obtiene o establece el patrón de recurrencia de la tarea recurrente. Puede ser uno de los valores de la enumeración [`RecurrencePattern`](./recurrencepattern/). |
| [TaskName](../../aspose.tasks/recurringtaskparameters/taskname/) { get; set; } | Obtiene o establece el nombre de la tarea recurrente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetCalendar](../../aspose.tasks/recurringtaskparameters/setcalendar/)(Project, string) | Establece un calendario para la tarea recurrente. El calendario se selecciona de la colección de calendarios del proyecto. |

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


