---
title: "AssignmentBaselineCollection.ParentAssignment"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα AssignmentBaselineCollection. Λαμβάνει το γονικό ResourceAssignment για αυτή τη συλλογή"
type: docs
weight: 30
url: /el/net/aspose.tasks/assignmentbaselinecollection/parentassignment/
---
## AssignmentBaselineCollection.ParentAssignment property

Λαμβάνει το γονικό [`ResourceAssignment`](../../resourceassignment/) για αυτή τη συλλογή.

```csharp
public ResourceAssignment ParentAssignment { get; }
```

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

* class [ResourceAssignment](../../resourceassignment/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


