---
title: "Prj.SplitsInProgressTasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, можно ли разбивать задачи в процессе выполнения"
type: docs
weight: 650
url: /ru/net/aspose.tasks/prj/splitsinprogresstasks/
---
## Prj.SplitsInProgressTasks field

Определяет, можно ли разделять задачи в процессе выполнения.

```csharp
public static readonly Key<NullableBool, PrjKey> SplitsInProgressTasks;
```

## Примеры

Показывает, как читать/записывать свойство Prj.SplitsInProgressTasks.

```csharp
var project = new Project();

project.Set(Prj.SplitsInProgressTasks, true);

Console.WriteLine("Splits In Progress Tasks: " + project.Get(Prj.SplitsInProgressTasks));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


