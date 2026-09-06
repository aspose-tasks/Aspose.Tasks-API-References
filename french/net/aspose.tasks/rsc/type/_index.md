---
title: "Rsc.Type"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le type d’une ressource"
type: docs
weight: 660
url: /fr/net/aspose.tasks/rsc/type/
---
## Rsc.Type field

Le type d'une ressource.

```csharp
public static readonly Key<ResourceType, RscKey> Type;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Type.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Type, ResourceType.Work);

Console.WriteLine("Type: " + resource.Get(Rsc.Type));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ResourceType](../../resourcetype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


