---
title: "Project.GetPredecessors"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método del proyecto. Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada"
type: docs
weight: 1120
url: /es/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Devuelve una colección de enlaces de tareas que son predecesores de la tarea especificada.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | La tarea para la cual obtener los predecesores. |

### Valor devuelto

Lista de predecesores [`TaskLink`](../../tasklink/).

## Ejemplos

Muestra cómo obtener los predecesores para una tarea específica.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Mostrar los nombres de las tareas predecesora y sucesora
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Ver también

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


