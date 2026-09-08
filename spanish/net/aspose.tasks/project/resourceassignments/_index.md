---
title: "Project.ResourceAssignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene el objeto ResourceAssignmentCollection"
type: docs
weight: 750
url: /es/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Obtiene el objeto ResourceAssignmentCollection.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Ejemplos

Muestra cómo trabajar con asignaciones de recursos.

```csharp
var project = new Project();

// Agregar nueva tarea y recurso
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Asignar el recurso a la tarea deseada
project.ResourceAssignments.Add(task, resource);
```

### Ver también

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


