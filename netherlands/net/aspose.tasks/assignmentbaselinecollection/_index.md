---
title: "Klasse AssignmentBaselineCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.AssignmentBaselineCollection class. Stelt een verzameling van AssignmentBaseline-objecten voor."
type: docs
weight: 60
url: /nl/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Stelt een verzameling van [`AssignmentBaseline`](../assignmentbaseline/) objecten voor.

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Haalt het aantal objecten op dat in dit AssignmentBaselineCollection-object zit. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Haalt de bovenliggende [`ResourceAssignment`](../resourceassignment/) op voor deze verzameling. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit. |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Verwijdert de baseline uit deze collectie. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Converteert het AssignmentBaselineCollection-object naar een lijst van [`AssignmentBaseline`](../assignmentbaseline/) objecten. |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


