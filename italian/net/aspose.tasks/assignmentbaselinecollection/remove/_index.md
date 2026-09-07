---
title: "AssignmentBaselineCollection.Remove"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo AssignmentBaselineCollection. Rimuove la baseline da questa collezione"
type: docs
weight: 60
url: /it/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Rimuove la baseline da questa raccolta.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | AssignmentBaseline | L'elemento da rimuovere. |

### Valore di ritorno

true se l'istanza di [`AssignmentBaseline`](../../assignmentbaseline/) è stata rimossa con successo; altrimenti, false

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


