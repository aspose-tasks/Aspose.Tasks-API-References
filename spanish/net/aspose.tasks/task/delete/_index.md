---
title: "Task.Delete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Task método. Elimina una tarea de la colección de tareas del proyecto padre y de todas sus asignaciones."
type: docs
weight: 1320
url: /es/net/aspose.tasks/task/delete/
---
## Task.Delete method

Elimina una tarea de la colección de tareas del proyecto principal y todas sus asignaciones.

```csharp
public void Delete()
```

## Ejemplos

Muestra cómo eliminar una tarea.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// eliminar una tarea
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


