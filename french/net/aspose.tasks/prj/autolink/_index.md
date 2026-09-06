---
title: "Prj.Autolink"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les tâches insérées ou déplacées sont automatiquement liées"
type: docs
weight: 70
url: /fr/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

Détermine si les tâches insérées ou déplacées sont automatiquement liées.

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## Exemples

Montre comment lire/écrire la propriété Prj.Autolink.

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


