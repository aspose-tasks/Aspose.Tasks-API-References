---
title: "Prj.SplitsInProgressTasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si les tâches en cours peuvent être fractionnées"
type: docs
weight: 650
url: /fr/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Détermine si les tâches en cours peuvent être fractionnées.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Exemples

Montre comment lire/écrire la propriété Prj.SplitsInProgressTasks.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


