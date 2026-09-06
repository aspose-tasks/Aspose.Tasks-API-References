---
title: "Rsc.Uid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L'identifiant unique d'une ressource"
type: docs
weight: 670
url: /fr/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

L'identifiant unique d'une ressource.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Uid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


