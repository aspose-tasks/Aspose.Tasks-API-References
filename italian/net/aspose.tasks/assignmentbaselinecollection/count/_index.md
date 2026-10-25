---
title: "AssignmentBaselineCollection.Count"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà AssignmentBaselineCollection. Ottiene il numero di oggetti contenuti in questo oggetto AssignmentBaselineCollection"
type: docs
weight: 10
url: /it/net/aspose.tasks/assignmentbaselinecollection/count/
---
## AssignmentBaselineCollection.Count property

Ottiene il numero di oggetti contenuti in questo oggetto AssignmentBaselineCollection.

```csharp
public int Count { get; }
```

## Esempi

Mostra come leggere le baseline di assegnazione.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// leggi le informazioni della baseline dell'assegnazione
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

// elimina le baseline di assegnazione
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Vedi anche

* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


