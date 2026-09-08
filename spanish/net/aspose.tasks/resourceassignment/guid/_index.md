---
title: "ResourceAssignment.Guid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment propiedad. Obtiene o establece un identificador único para esta asignación"
type: docs
weight: 290
url: /es/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Obtiene o establece el identificador único para esta asignación.

```csharp
public Guid? Guid { get; set; }
```

## Ejemplos

Muestra cómo leer un GUID de asignación de recurso.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### Ver también

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


