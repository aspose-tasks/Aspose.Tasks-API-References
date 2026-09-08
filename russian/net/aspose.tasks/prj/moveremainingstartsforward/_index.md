---
title: "Prj.MoveRemainingStartsForward"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, следует ли переместить начало оставшихся частей задач, запланированных к началу позже, к дате статуса"
type: docs
weight: 520
url: /ru/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

Определяет, следует ли переместить начало оставшихся частей задач, запланированных на более позднее начало, к дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## Примеры

Показывает, как читать/записывать свойство Prj.MoveRemainingStartsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


