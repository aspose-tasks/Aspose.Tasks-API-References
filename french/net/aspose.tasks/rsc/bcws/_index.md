---
title: "Rsc.BCWS"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le coût budgétaire d’un travail planifié pour une ressource"
type: docs
weight: 150
url: /fr/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

Le coût budgétaire d'un travail planifié pour une ressource.

```csharp
public static readonly Key<double, RscKey> BCWS;
```

## Exemples

Montre comment lire les coûts des ressources.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Afficher tous les coûts des ressources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


