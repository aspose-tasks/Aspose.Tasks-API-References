---
title: "Rsc.CostVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La différence entre le coût de référence et le coût total d’une ressource"
type: docs
weight: 250
url: /fr/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

La différence entre le coût de référence et le coût total pour une ressource.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.CostVariance.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


