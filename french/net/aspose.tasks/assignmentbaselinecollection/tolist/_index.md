---
title: "AssignmentBaselineCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode AssignmentBaselineCollection. Convertit l'objet AssignmentBaselineCollection en une liste d'objets AssignmentBaseline"
type: docs
weight: 70
url: /fr/net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

Convertit l'objet AssignmentBaselineCollection en une liste d'objets [`AssignmentBaseline`](../../assignmentbaseline/).

```csharp
public List<AssignmentBaseline> ToList()
```

### Valeur de retour

Liste d'objets [`AssignmentBaseline`](../../assignmentbaseline/).

## Exemples

Montre comment lire les lignes de base d'affectation.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// Lire les informations de ligne de base d'affectation
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

// supprimer les lignes de base d'affectation
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### Voir aussi

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


