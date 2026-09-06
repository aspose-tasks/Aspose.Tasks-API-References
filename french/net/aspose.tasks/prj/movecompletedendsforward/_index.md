---
title: "Prj.MoveCompletedEndsForward"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si la fin des parties terminées des tâches prévues comme terminées avant la date d'état mais commencées plus tard doit être avancée à la date d'état"
type: docs
weight: 500
url: /fr/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Détermine si la fin des parties terminées des tâches prévues comme terminées avant la date d'état mais commencées plus tard doit être avancée à la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


