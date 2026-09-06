---
title: "Rsc.Inactive"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si une ressource a été rendue inactive par un utilisateur disposant de droits administratifs"
type: docs
weight: 360
url: /fr/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

Détermine si une ressource a été rendue inactive par un utilisateur disposant de droits d'administrateur.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.Inactive.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


