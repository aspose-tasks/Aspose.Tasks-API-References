---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "AssignmentBaselineCollection μέθοδος. Αφαιρεί τη βάση από αυτή τη συλλογή"
type: docs
weight: 60
url: /el/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Αφαιρεί το baseline από αυτή τη συλλογή.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | AssignmentBaseline | Το στοιχείο προς αφαίρεση. |

### Τιμή Επιστροφής

αληθές εάν η παρουσία του [`AssignmentBaseline`](../../assignmentbaseline/) έχει αφαιρεθεί επιτυχώς· διαφορετικά, ψευδές

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


