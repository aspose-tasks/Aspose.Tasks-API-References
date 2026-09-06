---
title: "Resource.Baselines"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient une instance de BaselineCollection pour cet objet. Les valeurs de référence pour une ressource"
type: docs
weight: 160
url: /fr/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Obtient une instance de BaselineCollection pour cet objet. Les valeurs de référence pour une ressource.

```csharp
public BaselineCollection Baselines { get; }
```

## Exemples

Montre comment lire les repères d'une ressource.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Voir aussi

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


