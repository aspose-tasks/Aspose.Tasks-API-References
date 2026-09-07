---
title: "Prj.MoveCompletedEndsBack"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se la fine delle parti completate dei compiti programmati per iniziare dopo la data di stato ma iniziati prima debba essere riportata alla data di stato"
type: docs
weight: 490
url: /it/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Determina se la fine delle parti completate delle attività programmate per iniziare dopo la data di stato ma avviate prima debba essere riportata alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


