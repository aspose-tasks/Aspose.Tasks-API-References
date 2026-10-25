---
title: "Task.ParentTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene la tarea padre de una tarea"
type: docs
weight: 940
url: /es/net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Obtiene la tarea principal de una tarea.

```csharp
public Task ParentTask { get; }
```

## Ejemplos

Muestra cómo usar la tarea padre de una tarea.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


