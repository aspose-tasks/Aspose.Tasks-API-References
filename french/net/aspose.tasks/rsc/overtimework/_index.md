---
title: "Rsc.OvertimeWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le montant des heures supplémentaires programmées à être effectuées par une ressource sur une tâche et facturées aux taux d’heures supplémentaires des ressources concernées"
type: docs
weight: 530
url: /fr/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

Le montant des heures supplémentaires prévu pour être effectué par une ressource sur une tâche et facturé aux taux des heures supplémentaires des ressources concernées.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


