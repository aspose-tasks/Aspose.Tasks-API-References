---
title: "Rsc.ActualOvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Coûts engagés pour le travail supplémentaire déjà effectué sur les tâches par les ressources assignées"
type: docs
weight: 40
url: /fr/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Coûts engagés pour le travail supplémentaire déjà effectué sur les tâches par les ressources assignées.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.ActualOvertimeCost.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


