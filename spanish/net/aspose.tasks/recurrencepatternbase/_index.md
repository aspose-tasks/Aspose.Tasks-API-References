---
title: "Clase RecurrencePatternBase"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.RecurrencePatternBase. Representa la clase base del patrón de recurrencia"
type: docs
weight: 1700
url: /es/net/aspose.tasks/recurrencepatternbase/
---
## RecurrencePatternBase class

Representa la clase base del patrón de recurrencia.

```csharp
public abstract class RecurrencePatternBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Obtiene o establece el rango de recurrencia. |

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


