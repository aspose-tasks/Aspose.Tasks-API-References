---
title: "Prj.NewTasksAreManual"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, создаются ли новые задачи как ручные"
type: docs
weight: 550
url: /ru/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Определяет, создаются ли новые задачи как ручные.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Примеры

Показывает, как читать/записывать свойство Prj.NewTasksAreManual.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


