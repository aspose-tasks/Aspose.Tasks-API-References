---
title: "Prj.MoveCompletedEndsForward"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, следует ли переместить конец завершённых частей задач, запланированных к завершению до даты статуса, но начатых позже, до даты статуса"
type: docs
weight: 500
url: /ru/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Определяет, следует ли переместить конец завершённых частей задач, запланированных к завершению до даты статуса, но начавшихся позже, вперёд к дате статуса.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Примеры

Показывает, как читать/записывать свойство Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


