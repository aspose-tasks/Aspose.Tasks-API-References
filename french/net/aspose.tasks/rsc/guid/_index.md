---
title: "Rsc.Guid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Contient le code d’identification unique généré pour la ressource"
type: docs
weight: 310
url: /fr/net/aspose.tasks/rsc/guid/
---
## Rsc.Guid field

Contient le code d'identification unique généré pour la ressource.

```csharp
public static readonly Key<string, RscKey> Guid;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Guid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Guid, "1385689c-2dd1-4114-935b-054beb6fbbbe");

Console.WriteLine("Guid: " + resource.Get(Rsc.Guid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


