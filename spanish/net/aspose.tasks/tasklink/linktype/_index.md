---
title: "TaskLink.LinkType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskLink. Obtiene o establece el tipo de un enlace"
type: docs
weight: 60
url: /es/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Obtiene o establece el tipo de un enlace.

```csharp
public TaskLinkType LinkType { get; set; }
```

## Ejemplos

Muestra cómo obtener/establecer un tipo de enlace de un vínculo de tarea.

```csharp
var project = new Project();

// Agregar nuevas tareas
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Vincular tareas con el tipo de enlace establecido en Inicio a Inicio
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### Ver también

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


