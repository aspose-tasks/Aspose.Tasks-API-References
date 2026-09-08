---
title: "Clase RecurrenceRangeBase"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RecurrenceRangeBase. Representa el rango de recurrencia de una tarea recurrente."
type: docs
weight: 1710
url: /es/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

Representa el rango de recurrencia de una tarea recurrente.

```csharp
public abstract class RecurrenceRangeBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Obtiene o establece la fecha de inicio del rango de recurrencia de la tarea recurrente. |

## Ejemplos

Muestra cómo trabajar con repeticiones del patrón de repetición diaria al crear tareas recurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// trabaja con el proyecto más adelante...
// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


