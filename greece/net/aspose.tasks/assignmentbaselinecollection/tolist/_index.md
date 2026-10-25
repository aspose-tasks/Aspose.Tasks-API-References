---
title: "AssignmentBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "AssignmentBaselineCollection μέθοδος. Μετατρέπει το αντικείμενο AssignmentBaselineCollection σε λίστα αντικειμένων AssignmentBaseline"
type: docs
weight: 70
url: /el/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

Μετατρέπει το αντικείμενο AssignmentBaselineCollection σε λίστα αντικειμένων [`AssignmentBaseline`](../../assignmentbaseline/).

```csharp
public List<AssignmentBaseline> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων [`AssignmentBaseline`](../../assignmentbaseline/).

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


