---
title: "AssignmentBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα AssignmentBaselineCollection. Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο AssignmentBaselineCollection"
type: docs
weight: 10
url: /el/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο AssignmentBaselineCollection.

```csharp
public int Count { get; }
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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


