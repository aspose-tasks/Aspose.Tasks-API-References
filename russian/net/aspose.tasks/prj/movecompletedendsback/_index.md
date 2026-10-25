---
title: "Prj.MoveCompletedEndsBack"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, следует ли переместить конец завершённых частей задач, запланированных на начало после даты статуса, но начавшихся ранее, обратно к дате статуса"
type: docs
weight: 490
url: /ru/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Определяет, следует ли переместить конец завершённых частей задач, запланированных на начало после даты статуса, но начавшихся ранее, обратно к дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Примеры

Показывает, как читать/записывать свойство Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


