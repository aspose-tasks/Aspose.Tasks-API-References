---
title: "AssignmentBaselineCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode AssignmentBaselineCollection. Retourne un énumérateur pour cette collection"
type: docs
weight: 50
url: /fr/net/aspose.tasks/assignmentbaselinecollection/getenumerator/
---
## AssignmentBaselineCollection.GetEnumerator method

Renvoie un énumérateur pour cette collection.

```csharp
public IEnumerator<AssignmentBaseline> GetEnumerator()
```

### Valeur de retour

un énumérateur pour cette collection.

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


