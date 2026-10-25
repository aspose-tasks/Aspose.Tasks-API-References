---
title: "Rsc.CanLevel"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si l'équilibrage des ressources peut être effectué sur une ressource"
type: docs
weight: 200
url: /fr/net/aspose.tasks/rsc/canlevel/
---
## Rsc.CanLevel field

Détermine si le nivellement des ressources peut être effectué sur une ressource.

```csharp
public static readonly Key<NullableBool, RscKey> CanLevel;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.CanLevel.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CanLevel, true);

Console.WriteLine("Can Level: " + resource.Get(Rsc.CanLevel));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


