---
title: "Prj.MoveCompletedEndsBack"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si la fin des parties terminées des tâches planifiées pour commencer après la date d'état mais démarrées plus tôt doit être ramenée à la date d'état"
type: docs
weight: 490
url: /fr/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Détermine si la fin des parties terminées des tâches prévues pour commencer après la date d'état mais démarrées plus tôt doit être ramenée à la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


