---
title: "Rsc.IsCostResource"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si une ressource est une ressource de coût"
type: docs
weight: 390
url: /fr/net/aspose.tasks/rsc/iscostresource/
---
## Rsc.IsCostResource field

Détermine si une ressource est une ressource de coût.

```csharp
public static readonly Key<NullableBool, RscKey> IsCostResource;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsCostResource.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsCostResource, true);

Console.WriteLine("Is Cost Resource: " + resource.Get(Rsc.IsCostResource));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


