---
title: "Prj.RemoveFileProperties"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si toutes les propriétés de fichier seront supprimées lors de l'enregistrement"
type: docs
weight: 600
url: /fr/net/aspose.tasks/prj/removefileproperties/
---
## Prj.RemoveFileProperties field

Détermine si toutes les propriétés du fichier seront supprimées lors de l'enregistrement.

```csharp
public static readonly Key<NullableBool, PrjKey> RemoveFileProperties;
```

## Exemples

Montre comment lire/écrire la propriété Prj.RemoveFileProperties.

```csharp
var project = new Project();

project.Set(Prj.RemoveFileProperties, true);

Console.WriteLine("Remove File Properties: " + project.Get(Prj.RemoveFileProperties));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


