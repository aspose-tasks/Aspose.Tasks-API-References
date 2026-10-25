---
title: "AssignmentBaselineCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode AssignmentBaselineCollection. Supprime la ligne de base de cette collection"
type: docs
weight: 60
url: /fr/net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Supprime la ligne de base de cette collection.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | AssignmentBaseline | L'élément à supprimer. |

### Valeur de retour

true si l'instance [`AssignmentBaseline`](../../assignmentbaseline/) a été supprimée avec succès ; sinon, false

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


