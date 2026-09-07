---
title: "Κλάση AssignmentBaselineCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.AssignmentBaselineCollection. Αναπαριστά μια συλλογή αντικειμένων AssignmentBaseline."
type: docs
weight: 60
url: /el/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Αναπαριστά μια συλλογή αντικειμένων [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο AssignmentBaselineCollection. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Λαμβάνει τον γονέα [`ResourceAssignment`](../resourceassignment/) για αυτή τη συλλογή. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Αυτή είναι η ψευδοεφαρμογή της μεθόδου Add του ICollection, η οποία μόνο ρίχνει NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Αφαιρεί το baseline από αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Μετατρέπει το αντικείμενο AssignmentBaselineCollection σε λίστα αντικειμένων [`AssignmentBaseline`](../assignmentbaseline/). |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις βάσεις ανάθεσης.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// διαβάστε πληροφορίες βάσης ανάθεσης
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

// διαγραφή βάσεων ανάθεσης
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Δείτε επίσης

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


