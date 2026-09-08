---
title: "Prj.MoveRemainingStartsBack"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, следует ли перемещать начало оставшихся частей задач, запланированных на начало после даты статуса, но начатых ранее, обратно к дате статуса"
type: docs
weight: 510
url: /ru/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Определяет, следует ли переместить начало оставшихся частей задач, запланированных на начало после даты статуса, но начавшихся ранее, обратно к дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Примеры

Показывает, как читать/записывать свойство Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


