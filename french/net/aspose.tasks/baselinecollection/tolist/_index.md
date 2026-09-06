---
title: "BaselineCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode BaselineCollection. Convertit l'objet BaselineCollection en une liste d'objets Baseline"
type: docs
weight: 70
url: /fr/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Convertit l'objet BaselineCollection en une liste d'objets [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### Valeur de retour

Liste d'objets [`Baseline`](../../baseline/).

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


