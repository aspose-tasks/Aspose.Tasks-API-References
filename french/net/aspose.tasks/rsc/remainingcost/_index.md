---
title: "Rsc.RemainingCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La dépense prévue restante qui sera engagée lors de l'achèvement du travail prévu restant"
type: docs
weight: 580
url: /fr/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

La dépense prévue restante qui sera engagée pour terminer le travail prévu restant.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.RemainingCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


