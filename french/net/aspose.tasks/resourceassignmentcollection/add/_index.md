---
title: "ResourceAssignmentCollection.Add"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignmentCollection. Ajoute une nouvelle affectation à la ResourceAssignmentCollection"
type: docs
weight: 50
url: /fr/net/aspose.tasks/resourceassignmentcollection/add/
---
## Add(Task, Resource, double) {#add_1}

Ajoute une nouvelle affectation au ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, double units)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | Une tâche à affecter. |
| ressource | Ressource | Une ressource à affecter. |
| unités | Double | Le nombre d'unités pour une nouvelle affectation. |

### Valeur de retour

Affectation ajoutée.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource, decimal) {#add_2}

Ajoute une nouvelle affectation au ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, decimal cost)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | Une tâche à affecter. |
| ressource | Ressource | Une ressource de coût à affecter. |
| coût | Decimal | Le coût d'une nouvelle affectation. |

### Valeur de retour

Affectation ajoutée.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource) {#add}

Ajoute une nouvelle affectation au ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | Une tâche à affecter. |
| ressource | Ressource | Une ressource à affecter. |

### Valeur de retour

Affectation ajoutée.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(ResourceAssignment) {#add_3}

Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException

```csharp
public void Add(ResourceAssignment item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | ResourceAssignment | L'élément à supprimer. |

### Voir aussi

* class [ResourceAssignment](../../resourceassignment/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


