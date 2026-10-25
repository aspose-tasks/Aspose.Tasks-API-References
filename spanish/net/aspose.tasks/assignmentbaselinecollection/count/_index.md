---
title: "AssignmentBaselineCollection.Count"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad AssignmentBaselineCollection. Obtiene el número de objetos contenidos en este objeto AssignmentBaselineCollection"
type: docs
weight: 10
url: /es/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Obtiene el número de objetos contenidos en este objeto AssignmentBaselineCollection.

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


