---
title: "Rsc.Initials"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Les initiales d'une ressource"
type: docs
weight: 370
url: /fr/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

Les initiales d'une ressource.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Initials.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


