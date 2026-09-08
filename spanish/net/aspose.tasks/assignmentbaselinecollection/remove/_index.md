---
title: "AssignmentBaselineCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método AssignmentBaselineCollection. Elimina la línea base de esta colección"
type: docs
weight: 60
url: /es/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Elimina la línea base de esta colección.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | AssignmentBaseline | El elemento a eliminar. |

### Valor devuelto

true si la instancia de [`AssignmentBaseline`](../../assignmentbaseline/) se ha eliminado correctamente; de lo contrario, false

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


