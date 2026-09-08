---
title: "TaskLink.LinkLag"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskLink. Obtiene o establece el retraso en décimas de minuto o porcentaje"
type: docs
weight: 40
url: /es/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Obtiene o establece el retraso en décimas de minuto o en porcentaje.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


