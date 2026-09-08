---
title: "EndAfterRecurrenceRange.OccurrenceNumber"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad EndAfterRecurrenceRange. Obtiene o establece el número de ocurrencias que limita el rango de recurrencia de la tarea recurrente"
type: docs
weight: 20
url: /es/net/aspose.tasks/endafterrecurrencerange/occurrencenumber/
---
## EndAfterRecurrenceRange.OccurrenceNumber property

Obtiene o establece el número de ocurrencias que limita el rango de recurrencia de la tarea recurrente.

```csharp
public int OccurrenceNumber { get; set; }
```

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

* class [EndAfterRecurrenceRange](../)
* namespace [Aspose.Tasks](../../endafterrecurrencerange/)
* assembly [Aspose.Tasks](../../../)


