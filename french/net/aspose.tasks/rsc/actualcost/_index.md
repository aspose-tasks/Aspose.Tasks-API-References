---
title: "Rsc.ActualCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches ainsi que tout autre coût enregistré associé à la tâche"
type: docs
weight: 30
url: /fr/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Coûts engagés pour le travail déjà effectué par les ressources sur leurs tâches, ainsi que tous les autres coûts enregistrés associés à la tâche.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


