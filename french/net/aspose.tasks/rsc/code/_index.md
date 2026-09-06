---
title: "Rsc.Code"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le code ou d'autres informations concernant une ressource"
type: docs
weight: 210
url: /fr/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

Le code ou d'autres informations concernant une ressource.

```csharp
public static readonly Key<string, RscKey> Code;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Code.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


