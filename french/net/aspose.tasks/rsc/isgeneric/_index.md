---
title: "Rsc.IsGeneric"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si une ressource est générique ou non"
type: docs
weight: 410
url: /fr/net/aspose.tasks/rsc/isgeneric/
---
## Rsc.IsGeneric field

Détermine si une ressource est générique ou non.

```csharp
public static readonly Key<NullableBool, RscKey> IsGeneric;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsGeneric.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsGeneric, true);

Console.WriteLine("Is Generic: " + resource.Get(Rsc.IsGeneric));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


