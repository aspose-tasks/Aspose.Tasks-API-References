---
title: "Clase TaskLink"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskLink. Representa un enlace de predecesor"
type: docs
weight: 2410
url: /es/net/aspose.tasks/tasklink/
---
## TaskLink class

Representa un enlace de predecesor.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Obtiene o establece el proyecto predecesor externo. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Obtiene o establece un valor que indica si un predecesor forma parte de otro proyecto. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Obtiene o establece el formato para expresar el retraso. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Obtiene o establece el retraso en décimas de minuto o en porcentaje. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Obtiene o establece la duración del retraso, según LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Obtiene o establece el tipo de un enlace. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Obtiene o establece la tarea predecesora. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Obtiene o establece la tarea sucesora. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `TaskLink`. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Devuelve la representación en cadena de un TaskLink. Los detalles exactos de la representación no están especificados y pueden cambiar. |

## Ejemplos

Muestra cómo leer los enlaces de tareas del proyecto.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Mostrar los nombres de las tareas predecesora y sucesora
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


