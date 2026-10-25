---
title: "Task.Status"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene el estado de la tarea"
type: docs
weight: 1160
url: /es/net/aspose.tasks/task/status/
---
## Task.Status property

Obtiene el estado de la tarea.

```csharp
public TaskStatus Status { get; }
```

## Ejemplos

Muestra cómo obtener el estado de la tarea.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// La fecha de estado del proyecto debe establecerse porque el cálculo del estado utiliza la fecha de estado.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Ver también

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


