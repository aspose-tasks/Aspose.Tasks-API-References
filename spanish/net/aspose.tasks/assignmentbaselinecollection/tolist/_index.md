---
title: "AssignmentBaselineCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método AssignmentBaselineCollection. Convierte el objeto AssignmentBaselineCollection a una lista de objetos AssignmentBaseline"
type: docs
weight: 70
url: /es/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

Convierte el objeto AssignmentBaselineCollection a una lista de objetos [`AssignmentBaseline`](../../assignmentbaseline/).

```csharp
public List<AssignmentBaseline> ToList()
```

### Valor devuelto

Lista de objetos [`AssignmentBaseline`](../../assignmentbaseline/).

## Ejemplos

Muestra cómo leer líneas base de asignación.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// leer información de la línea base de asignación
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// eliminar líneas base de asignación
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Ver también

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


