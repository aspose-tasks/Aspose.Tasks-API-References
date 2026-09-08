---
title: "AssignmentBaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AssignmentBaselineCollection methode. Verwijdert de baseline uit deze collectie"
type: docs
weight: 60
url: /nl/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Verwijdert de baseline uit deze collectie.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | AssignmentBaseline | Het item om te verwijderen. |

### Retourwaarde

true als [`AssignmentBaseline`](../../assignmentbaseline/) instantie succesvol is verwijderd; anders, false

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


