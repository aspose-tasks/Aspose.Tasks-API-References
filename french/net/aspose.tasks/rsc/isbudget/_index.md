---
title: "Rsc.IsBudget"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Détermine si un matériau de travail ou une ressource de coût est une ressource budgétaire"
type: docs
weight: 380
url: /fr/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

Détermine si une ressource de travail, de matériel ou de coût est une ressource budgétaire.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## Exemples

Montre comment lire/écrire la propriété Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


