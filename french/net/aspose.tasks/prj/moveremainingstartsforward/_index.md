---
title: "Prj.MoveRemainingStartsForward"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si le début des parties restantes des tâches prévues pour commencer plus tard doit être avancé à la date d'état"
type: docs
weight: 520
url: /fr/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Détermine si le début des parties restantes des tâches planifiées pour avoir commencé plus tard doit être avancé jusqu'à la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


