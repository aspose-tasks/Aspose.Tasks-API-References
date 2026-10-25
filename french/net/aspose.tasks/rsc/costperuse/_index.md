---
title: "Rsc.CostPerUse"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le coût qui s’accumule chaque fois qu’une ressource est utilisée"
type: docs
weight: 240
url: /fr/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

Le coût qui s'accumule chaque fois qu'une ressource est utilisée.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.CostPerUse.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


