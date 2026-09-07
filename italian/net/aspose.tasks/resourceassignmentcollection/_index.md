---
title: "Classe ResourceAssignmentCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ResourceAssignmentCollection. Rappresenta una raccolta di oggetti ResourceAssignment"
type: docs
weight: 1760
url: /it/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Rappresenta una raccolta di oggetti [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Ottiene il numero di oggetti contenuti nella ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Ottiene il progetto genitore dell'oggetto ResourceAssignmentCollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Aggiunge una nuova assegnazione alla ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Restituisce un'assegnazione con l'uid specificato. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Rimuove l'assegnazione specificata dalla raccolta, se non è di sola lettura, altrimenti genera NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Rimuove l'assegnazione all'indice specificato, se la raccolta non è di sola lettura, altrimenti genera NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Converte l'oggetto ResourceAssignmentCollection in un elenco di oggetti [`ResourceAssignment`](../resourceassignment/). |

## Esempi

Mostra come lavorare con le raccolte di assegnazioni di risorse.

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

// lavorare con l'assegnazione...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// converti la raccolta in una lista
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// itera sulla lista
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Vedi anche

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


