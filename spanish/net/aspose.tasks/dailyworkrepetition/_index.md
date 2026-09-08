---
title: "Clase DailyWorkRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.DailyWorkRepetition. Representa una clase para repeticiones en el patrón de recurrencia diaria basado en días laborables"
type: docs
weight: 420
url: /es/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Representa una clase para repeticiones en un patrón de recurrencia diaria basado en días laborables.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Inicializa una nueva instancia de la clase `DailyWorkRepetition`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Obtiene o establece un número de días que representa el intervalo en días entre ocurrencias. |

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

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


