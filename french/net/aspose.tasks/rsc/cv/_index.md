---
title: "Rsc.CV"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La variance du coût de la valeur acquise jusqu’à la date d’état du projet. CV est la différence entre le BCWP (coût budgété du travail réalisé) des tâches et l’ACWP (coût réel du travail réalisé)."
type: docs
weight: 270
url: /fr/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

L'écart de coût de la valeur acquise, à la date d'état du projet. CV est la différence entre le BCWP (coût budgété du travail effectué) et l'ACWP (coût réel du travail effectué) de la tâche.

```csharp
public static readonly Key<double, RscKey> CV;
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


