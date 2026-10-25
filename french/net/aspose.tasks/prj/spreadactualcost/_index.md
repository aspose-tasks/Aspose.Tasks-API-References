---
title: "Prj.SpreadActualCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les coûts réels sont répartis jusqu'à la date d'état"
type: docs
weight: 660
url: /fr/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

Détermine si les coûts réels sont répartis jusqu'à la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## Exemples

Montre comment lire/écrire la propriété Prj.SpreadActualCost.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


