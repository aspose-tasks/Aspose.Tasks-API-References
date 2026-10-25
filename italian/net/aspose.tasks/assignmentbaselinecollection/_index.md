---
title: "Classe AssignmentBaselineCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.AssignmentBaselineCollection. Rappresenta una raccolta di oggetti AssignmentBaseline"
type: docs
weight: 60
url: /it/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Rappresenta una raccolta di oggetti [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto AssignmentBaselineCollection. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Ottiene il genitore [`ResourceAssignment`](../resourceassignment/) per questa raccolta. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Rimuove la baseline da questa raccolta. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Converte l'oggetto AssignmentBaselineCollection in un elenco di oggetti [`AssignmentBaseline`](../assignmentbaseline/). |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


