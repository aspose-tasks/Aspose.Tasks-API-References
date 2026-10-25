---
title: "Rsc.SV"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La variance d'échéancier de la valeur acquise jusqu'à la date d'état du projet. SV est la différence entre le coût budgété du travail effectué (BCWP) et le coût budgété du travail programmé (BCWS)"
type: docs
weight: 650
url: /fr/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

La variance d'échéancier de la valeur acquise, jusqu'à la date d'état du projet. SV est la différence entre le coût budgété du travail effectué (BCWP) et le coût budgété du travail prévu (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


