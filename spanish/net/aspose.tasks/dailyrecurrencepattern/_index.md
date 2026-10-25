---
title: "Clase DailyRecurrencePattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.DailyRecurrencePattern. Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente diaria en un proyecto."
type: docs
weight: 400
url: /es/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Representa el conjunto de parámetros que se utilizan para crear una tarea recurrente diaria en un proyecto.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Inicializa una nueva instancia de la clase `DailyRecurrencePattern`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtiene o establece el rango de recurrencia. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Obtiene o establece el patrón de repeticiones en el patrón de recurrencia diaria. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


