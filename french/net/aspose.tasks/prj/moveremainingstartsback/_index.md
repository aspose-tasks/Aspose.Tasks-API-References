---
title: "Prj.MoveRemainingStartsBack"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Détermine si le début des parties restantes des tâches planifiées pour commencer après la date d’état mais démarrées plus tôt doit être ramené à la date d’état"
type: docs
weight: 510
url: /fr/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Détermine si le début des parties restantes des tâches planifiées pour commencer après la date d'état mais commencées plus tôt doit être déplacé vers la date d'état.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Exemples

Montre comment lire/écrire la propriété Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


