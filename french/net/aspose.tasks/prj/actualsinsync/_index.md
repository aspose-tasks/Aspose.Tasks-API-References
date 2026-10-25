---
title: "Prj.ActualsInSync"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si tous les travaux réels ont été synchronisés avec le projet"
type: docs
weight: 10
url: /fr/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

Détermine si tous les travaux réels ont été synchronisés avec le projet.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## Exemples

Montre comment lire/écrire la propriété Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


