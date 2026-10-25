---
title: "Klasse ResourceAssignmentCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ResourceAssignmentCollection‑klasse. Vertegenwoordigt een collectie van ResourceAssignment‑objecten"
type: docs
weight: 1760
url: /nl/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Vertegenwoordigt een collectie van [`ResourceAssignment`](../resourceassignment/) objecten.

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Haalt het aantal objecten op dat in de ResourceAssignmentCollection zit. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Geeft een waarde terug die aangeeft of deze collectie alleen‑lezen is. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Haalt het bovenliggende project op van het ResourceAssignmentCollection‑object. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Retourneert een toewijzing met de opgegeven uid. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Verwijdert de opgegeven toewijzing uit de collectie, als deze niet alleen‑lezen is; anders wordt een NotSupportedException gegooid. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Verwijdert de toewijzing op de opgegeven index, als de collectie niet alleen‑lezen is; anders wordt een NotSupportedException gegooid. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Converteert het ResourceAssignmentCollection‑object naar een lijst van [`ResourceAssignment`](../resourceassignment/) objecten. |

## Voorbeelden

Toont hoe te werken met collecties van resource‑toewijzingen.

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

// werken met toewijzing...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// converteer de collectie naar een lijst
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// itereren over de lijst
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Zie ook

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


