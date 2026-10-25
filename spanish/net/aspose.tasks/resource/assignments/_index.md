---
title: "Resource.Assignments"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Resource. Obtiene una colección de asignaciones de recursos para este objeto"
type: docs
weight: 120
url: /es/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Obtiene una colección de asignaciones de recursos para este objeto.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Ejemplos

Muestra cómo leer asignaciones de un recurso.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### Ver también

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


