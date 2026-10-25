---
title: "BaselineCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode BaselineCollection. Supprime le baseline de cette collection"
type: docs
weight: 60
url: /fr/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Supprime la ligne de base de cette collection.

```csharp
public bool Remove(Baseline item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | Baseline | L'élément à supprimer. |

### Valeur de retour

true si l'instance [`Baseline`](../../baseline/) a été supprimée avec succès ; sinon, false

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


