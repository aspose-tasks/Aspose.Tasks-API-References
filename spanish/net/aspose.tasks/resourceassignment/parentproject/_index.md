---
title: "ResourceAssignment.ParentProject"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ResourceAssignment. Obtiene el proyecto principal para esta asignación"
type: docs
weight: 420
url: /es/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Obtiene el proyecto principal para esta asignación.

```csharp
public Project ParentProject { get; }
```

## Ejemplos

Muestra cómo usar el proyecto principal de una asignación de recursos.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// establece una duración de la asignación usando el tipo de unidad de tiempo predeterminado del proyecto.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### Ver también

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


