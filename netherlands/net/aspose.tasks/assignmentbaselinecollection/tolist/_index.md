---
title: "AssignmentBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentBaselineCollection methode. Converteert het AssignmentBaselineCollection-object naar een lijst van AssignmentBaseline-objecten"
type: docs
weight: 70
url: /nl/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

Converteert het AssignmentBaselineCollection-object naar een lijst van [`AssignmentBaseline`](../../assignmentbaseline/) objecten.

```csharp
public List<AssignmentBaseline> ToList()
```

### Retourwaarde

Lijst van [`AssignmentBaseline`](../../assignmentbaseline/) objecten.

## Voorbeelden

Toont hoe toewijzingsbaselines gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// lees toewijzingsbaseline‑informatie
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

// verwijder toewijzingsbaselines
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Zie ook

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


