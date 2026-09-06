---
title: "Rsc.Cost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le coût total programmé ou prévu pour une ressource, basé sur les coûts déjà engagés pour le travail effectué par les ressources affectées aux tâches, ainsi que sur les coûts prévus pour le travail restant."
type: docs
weight: 220
url: /fr/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Le coût total planifié ou projeté pour une ressource, basé sur les coûts déjà engagés pour le travail effectué par les ressources affectées aux tâches, ainsi que sur les coûts prévus pour le travail restant.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


