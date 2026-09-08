---
title: "Task.Successors"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene un objeto TaskCollection que contiene todos los sucesores de este objeto Task"
type: docs
weight: 1200
url: /es/net/aspose.tasks/task/successors/
---
## Task.Successors property

Obtiene un objeto [`TaskCollection`](../../taskcollection/) que contiene todos los sucesores de este objeto Task.

```csharp
public TaskCollection Successors { get; }
```

### Valor devuelto

Instancia de solo lectura de la clase [`TaskCollection`](../../taskcollection/).

## Ejemplos

Muestra cómo leer los sucesores de la tarea.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Ver también

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


