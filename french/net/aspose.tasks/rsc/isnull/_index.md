---
title: "Rsc.IsNull"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si une ressource est nulle"
type: docs
weight: 420
url: /fr/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

Détermine si une ressource est nulle.

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsNull.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


