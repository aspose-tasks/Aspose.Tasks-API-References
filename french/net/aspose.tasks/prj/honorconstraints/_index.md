---
title: "Prj.HonorConstraints"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les tâches respectent leurs dates de contrainte"
type: docs
weight: 370
url: /fr/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

Détermine si les tâches respectent leurs dates de contrainte.

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## Exemples

Montre comment lire/écrire la propriété Prj.HonorConstraints.

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


