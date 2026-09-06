---
title: "Rsc.RemainingOvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La dépense d’heures supplémentaires prévue restante pour une ressource"
type: docs
weight: 590
url: /fr/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

La dépense supplémentaire prévue restante pour une ressource.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.RemainingOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


