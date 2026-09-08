---
title: "ResourceAssignment.Delete"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment método. Elimina la asignación de recursos de la colección de asignaciones del proyecto"
type: docs
weight: 680
url: /es/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Elimina la asignación de recursos de la colección de asignaciones del proyecto.

```csharp
public void Delete()
```

## Ejemplos

Muestra cómo eliminar una asignación de recursos.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


