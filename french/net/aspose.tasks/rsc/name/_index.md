---
title: "Rsc.Name"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le nom d'une ressource"
type: docs
weight: 460
url: /fr/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

Le nom d'une ressource.

```csharp
public static readonly Key<string, RscKey> Name;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Name.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


