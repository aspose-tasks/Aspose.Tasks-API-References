---
title: "Task.Predecessors"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene un objeto TaskCollection que contiene todos los predecesores de este objeto Task"
type: docs
weight: 980
url: /es/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Obtiene un objeto [`TaskCollection`](../../taskcollection/) que contiene todos los predecesores de este objeto Task.

```csharp
public TaskCollection Predecessors { get; }
```

### Valor devuelto

Instancia de solo lectura de la clase [`TaskCollection`](../../taskcollection/).

## Ejemplos

Muestra cómo leer los predecesores de la tarea.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Ver también

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


