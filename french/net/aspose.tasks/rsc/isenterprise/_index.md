---
title: "Rsc.IsEnterprise"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Indique si une ressource provient du pool de ressources d'entreprise (vrai) ou du pool de ressources local (faux)"
type: docs
weight: 400
url: /fr/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Indique si une ressource provient du pool de ressources d'entreprise (vrai) ou du pool de ressources local (faux).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


