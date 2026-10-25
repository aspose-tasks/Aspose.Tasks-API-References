---
title: "Prj.MoveCompletedEndsForward"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Prj field. Determina se la fine delle parti completate delle attività programmate per essere completate prima della data di stato ma iniziate più tardi debba essere spostata alla data di stato"
type: docs
weight: 500
url: /it/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Determina se la fine delle parti completate delle attività programmate per essere completate prima della data di stato ma avviate più tardi debba essere spostata in avanti alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


