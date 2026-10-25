---
title: "TaskLink.PredTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskLink. Obtiene o establece la tarea predecesora"
type: docs
weight: 70
url: /es/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Obtiene o establece la tarea predecesora.

```csharp
public Task PredTask { get; set; }
```

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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


