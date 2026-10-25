---
title: "Clase AssignmentBaselineCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.AssignmentBaselineCollection clase. Representa una colección de objetos AssignmentBaseline."
type: docs
weight: 60
url: /es/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Representa una colección de objetos [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Obtiene el número de objetos contenidos en este objeto AssignmentBaselineCollection. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Obtiene el padre [`ResourceAssignment`](../resourceassignment/) de esta colección. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Elimina la línea base de esta colección. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Convierte el objeto AssignmentBaselineCollection a una lista de objetos [`AssignmentBaseline`](../assignmentbaseline/). |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


