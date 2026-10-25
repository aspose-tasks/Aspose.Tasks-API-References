---
title: "AssignmentBaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentBaselineCollection-eigenschap. Haalt het aantal objecten op dat in dit AssignmentBaselineCollection‑object zit"
type: docs
weight: 10
url: /nl/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Haalt het aantal objecten op dat in dit AssignmentBaselineCollection-object zit.

```csharp
public int Count { get; }
```

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

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


