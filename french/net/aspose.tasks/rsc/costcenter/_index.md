---
title: "Rsc.CostCenter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Indique à quel centre de coûts les dépenses accumulées par la ressource doivent être imputées"
type: docs
weight: 230
url: /fr/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Indique à quel centre de coûts les coûts accumulés par la ressource doivent être imputés.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.CostCenter.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


