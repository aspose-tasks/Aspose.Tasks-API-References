---
title: "Rsc.OvertimeRateFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Les unités utilisées par Microsoft Project pour afficher le taux d’heures supplémentaires"
type: docs
weight: 520
url: /fr/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Les unités utilisées par Microsoft Project pour afficher le taux des heures supplémentaires.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


