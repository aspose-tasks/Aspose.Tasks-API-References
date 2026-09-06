---
title: "Classe BaselineCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.BaselineCollection. Représente une collection d'objets Baseline"
type: docs
weight: 120
url: /fr/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Représente une collection d'objets [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet BaselineCollection. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Renvoie l'élément à l'index spécifié. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Obtient le parent [`Resource`](../resource/) de cette collection. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Supprime la ligne de base de cette collection. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Convertit l'objet BaselineCollection en une liste d'objets [`Baseline`](../baseline/). |

## Exemples

Montre comment travailler avec les collections de lignes de base.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// lire les informations de la ligne de base
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### Voir aussi

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


