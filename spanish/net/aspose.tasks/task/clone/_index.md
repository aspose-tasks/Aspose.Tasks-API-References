---
title: "Task.Clone"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Task. Crea una copia completa de una tarea sin subtareas"
type: docs
weight: 1310
url: /es/net/aspose.tasks/task/clone/
---
## Task.Clone method

Crea una copia completa de una tarea sin subtareas.

```csharp
public object Clone()
```

### Valor devuelto

Copia creada de una tarea.

## Ejemplos

Muestra cómo clonar una tarea.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


