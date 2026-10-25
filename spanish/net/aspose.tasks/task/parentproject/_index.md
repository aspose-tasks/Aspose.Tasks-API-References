---
title: "Task.ParentProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Task. Obtiene el proyecto padre de una tarea"
type: docs
weight: 930
url: /es/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Obtiene el proyecto principal de una tarea.

```csharp
public Project ParentProject { get; }
```

## Observaciones

Llame a Project.UpdateReferences para actualizar estas propiedades.

## Ejemplos

Muestra cómo usar el proyecto padre de la tarea.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// establezca una duración para la tarea usando el tipo de unidad de tiempo predeterminado del proyecto.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### Ver también

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


