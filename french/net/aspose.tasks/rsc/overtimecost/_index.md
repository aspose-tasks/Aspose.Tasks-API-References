---
title: "Rsc.OvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le coût total des heures supplémentaires pour une ressource sur toutes les tâches assignées"
type: docs
weight: 500
url: /fr/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Le coût total des heures supplémentaires pour une ressource sur toutes les tâches assignées.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Exemples

Montre comment lire les valeurs d'heures supplémentaires de la ressource.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Afficher les paramètres liés aux heures supplémentaires pour toutes les ressources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


