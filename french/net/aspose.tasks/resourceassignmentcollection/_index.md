---
title: "Classe ResourceAssignmentCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.ResourceAssignmentCollection. Représente une collection d'objets ResourceAssignment."
type: docs
weight: 1760
url: /fr/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Représente une collection d'objets [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Obtient le nombre d'objets contenus dans le ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Obtient le projet parent de l'objet ResourceAssignmentCollection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Ajoute une nouvelle affectation au ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Ajoute une nouvelle affectation au ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Ajoute une nouvelle affectation au ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Renvoie une affectation avec l'uid spécifié. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Supprime l'affectation spécifiée de la collection, si elle n'est pas en lecture seule, sinon lève NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Supprime l'affectation à l'index spécifié, si la collection n'est pas en lecture seule, sinon lève NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Convertit l'objet ResourceAssignmentCollection en une liste d'objets [`ResourceAssignment`](../resourceassignment/). |

## Exemples

Montre comment travailler avec les collections d'affectations de ressources.

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

// travailler avec l'affectation...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convertir la collection en une liste
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// itérer sur la liste
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Voir aussi

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


