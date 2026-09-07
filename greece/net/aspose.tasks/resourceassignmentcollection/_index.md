---
title: "Κλάση ResourceAssignmentCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.ResourceAssignmentCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων ResourceAssignment."
type: docs
weight: 1760
url: /el/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται στη ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Λαμβάνει το γονικό έργο του αντικειμένου ResourceAssignmentCollection. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Αυτή είναι η ψευδοεφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Προσθέτει νέα ανάθεση στη ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Προσθέτει νέα ανάθεση στη ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Προσθέτει νέα ανάθεση στη ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Επιστρέφει μια ανάθεση με το καθορισμένο uid. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Αφαιρεί την καθορισμένη ανάθεση από τη συλλογή, εάν δεν είναι μόνο για ανάγνωση, διαφορετικά ρίχνει NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Αφαιρεί την ανάθεση στο καθορισμένο δείκτη, εάν η συλλογή δεν είναι μόνο για ανάγνωση, διαφορετικά ρίχνει NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Μετατρέπει το αντικείμενο ResourceAssignmentCollection σε λίστα αντικειμένων [`ResourceAssignment`](../resourceassignment/). |

## Παραδείγματα

Εμφανίζει πώς να εργαστείτε με συλλογές αναθέσεων πόρων.

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

// εργαστείτε με ανάθεση...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// μετατρέψτε τη συλλογή σε λίστα
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// επανάληψη στη λίστα
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Δείτε επίσης

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


