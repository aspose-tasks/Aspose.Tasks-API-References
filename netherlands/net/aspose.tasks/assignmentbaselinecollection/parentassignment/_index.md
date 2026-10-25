---
title: "AssignmentBaselineCollection.ParentAssignment"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentBaselineCollection-eigenschap. Haalt de bovenliggende ResourceAssignment voor deze collectie op"
type: docs
weight: 30
url: /nl/net/aspose.tasks/assignmentbaselinecollection/parentassignment/
---
## AssignmentBaselineCollection.ParentAssignment property

Haalt de bovenliggende [`ResourceAssignment`](../../resourceassignment/)-object op voor deze collectie.

```csharp
public ResourceAssignment ParentAssignment { get; }
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

* class [ResourceAssignment](../../resourceassignment/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


