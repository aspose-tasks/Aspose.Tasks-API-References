---
title: "Project.TaskLinks"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene el objeto TaskLinkCollection."
type: docs
weight: 930
url: /es/net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Obtiene el objeto [`TaskLinkCollection`](../../tasklinkcollection/).

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Ejemplos

Muestra cómo crear enlaces de tareas.

```csharp
var project = new Project();

// Agregar nuevas tareas
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Vincular tareas
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### Ver también

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


