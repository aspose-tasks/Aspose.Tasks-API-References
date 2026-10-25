---
title: "Clase ResourceAssignmentCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ResourceAssignmentCollection. Representa una colección de objetos ResourceAssignment"
type: docs
weight: 1760
url: /es/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Representa una colección de objetos [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Obtiene el número de objetos contenidos en ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Devuelve el elemento en el índice especificado. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Obtiene el proyecto principal del objeto ResourceAssignmentCollection. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Agrega una nueva asignación a ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Agrega una nueva asignación a ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Agrega una nueva asignación a ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Devuelve una asignación con el uid especificado. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Elimina la asignación especificada de la colección, si no es de solo lectura; de lo contrario, lanza NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Elimina la asignación en el índice especificado, si la colección no es de solo lectura; de lo contrario, lanza NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Convierte el objeto ResourceAssignmentCollection en una lista de objetos [`ResourceAssignment`](../resourceassignment/). |

## Ejemplos

Muestra cómo trabajar con colecciones de asignaciones de recursos.

```csharp
var project = new Project(DataDir + "TemplateResource2010.mpp");

var task = project.RootTask.Children.Add("Task 1");
var resource = project.Resources.Add("Resource 1");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignment.Set(Asn.Work, project.GetWork(40));
assignment.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithUnits = project.ResourceAssignments.Add(task, resource, 1d);
assignmentWithUnits.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithUnits.Set(Asn.Work, project.GetWork(40));
assignmentWithUnits.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithCost = project.ResourceAssignments.Add(task, resource);
assignmentWithCost.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithCost.Set(Asn.Work, project.GetWork(40));
assignmentWithCost.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

Console.WriteLine("Print assignments for the project: " + project.ResourceAssignments.ParentProject.Get(Prj.Name));
Console.WriteLine("Resource assignment count: " + project.ResourceAssignments.Count);
foreach (var resourceAssignment in project.ResourceAssignments)
{
    Console.WriteLine("Task Name: " + resourceAssignment.Get(Asn.Task).Get(Tsk.Name));
    Console.WriteLine("Uid: " + resourceAssignment.Get(Asn.Uid));
    Console.WriteLine("Start: " + resourceAssignment.Get(Asn.Start));
    Console.WriteLine("Work: " + resourceAssignment.Get(Asn.Work));
    Console.WriteLine("Finish: " + resourceAssignment.Get(Asn.Finish));
}

var assignmentByUid = project.ResourceAssignments.GetByUid(2);
Console.WriteLine("Assignment By Uid Start: " + assignmentByUid.Get(Asn.Start));

// trabajar con asignaciones...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convertir la colección en una lista
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// iterar sobre la lista
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Ver también

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


