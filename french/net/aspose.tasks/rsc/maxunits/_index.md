---
title: "Rsc.MaxUnits"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le nombre maximal d’unités représentant la capacité maximale pour laquelle une ressource est disponible afin d’accomplir des tâches pendant la période actuelle"
type: docs
weight: 450
url: /fr/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

Le nombre maximal d'unités représentant la capacité maximale pour laquelle une ressource est disponible afin d'accomplir des tâches pendant la période actuelle.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.MaxUnits.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


