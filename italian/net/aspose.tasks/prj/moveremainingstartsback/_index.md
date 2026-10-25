---
title: "Prj.MoveRemainingStartsBack"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare dopo la data di stato ma avviate in anticipo debba essere riportato alla data di stato."
type: docs
weight: 510
url: /it/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Determina se l'inizio delle parti rimanenti delle attività programmate per iniziare dopo la data di stato ma avviate prima debba essere riportato alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


