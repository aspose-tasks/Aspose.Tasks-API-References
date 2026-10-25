---
title: "Prj.MultipleCriticalPaths"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si plusieurs chemins critiques sont calculés"
type: docs
weight: 530
url: /fr/net/aspose.tasks/prj/multiplecriticalpaths/
---
## Prj.MultipleCriticalPaths field

Détermine si plusieurs chemins critiques sont calculés.

```csharp
public static readonly Key<NullableBool, PrjKey> MultipleCriticalPaths;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MultipleCriticalPaths.

```csharp
var project = new Project();

project.Set(Prj.MultipleCriticalPaths, true);

Console.WriteLine("Multiple Critical Paths: " + project.Get(Prj.MultipleCriticalPaths));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


