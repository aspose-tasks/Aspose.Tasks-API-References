---
title: "Prj.MoveRemainingStartsForward"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare più tardi debba essere anticipato alla data di stato"
type: docs
weight: 520
url: /it/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare più tardi debba essere anticipato alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


