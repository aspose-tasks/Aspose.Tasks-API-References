---
title: "AssignmentBaselineCollection.GetEnumerator"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo AssignmentBaselineCollection. Restituisce un enumeratore per questa collezione"
type: docs
weight: 50
url: /it/net/aspose.tasks/assignmentbaselinecollection/getenumerator/
---
## AssignmentBaselineCollection.GetEnumerator method

Restituisce un enumeratore per questa collezione.

```csharp
public IEnumerator<AssignmentBaseline> GetEnumerator()
```

### Valore di ritorno

un enumeratore per questa collezione.

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

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


