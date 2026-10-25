---
title: "Rsc.Id"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. L'identifiant de position d'une ressource dans la liste des ressources"
type: docs
weight: 350
url: /fr/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

L'identifiant de position d'une ressource dans la liste des ressources.

```csharp
public static readonly Key<int, RscKey> Id;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Id.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


