---
title: "Classe AssignmentBaselineCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.AssignmentBaselineCollection. Représente une collection d'objets AssignmentBaseline."
type: docs
weight: 60
url: /fr/net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Représente une collection d'objets [`AssignmentBaseline`](../assignmentbaseline/).

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet AssignmentBaselineCollection. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Obtient le parent [`ResourceAssignment`](../resourceassignment/) de cette collection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Supprime la ligne de base de cette collection. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Convertit l'objet AssignmentBaselineCollection en une liste d'objets [`AssignmentBaseline`](../assignmentbaseline/). |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


