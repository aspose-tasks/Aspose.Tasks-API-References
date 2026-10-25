---
title: "Prj.NewTasksEffortDriven"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, являются ли новые задачи зависимыми от усилий"
type: docs
weight: 560
url: /ru/net/aspose.tasks/prj/newtaskseffortdriven/
---
## Prj.NewTasksEffortDriven field

Определяет, являются ли новые задачи ориентированными на трудозатраты.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEffortDriven;
```

## Примеры

Показывает, как читать/записывать свойство Prj.NewTasksEffortDriven.

```csharp
var project = new Project();

project.Set(Prj.NewTasksEffortDriven, true);

Console.WriteLine("New Tasks Effort Driven: " + project.Get(Prj.NewTasksEffortDriven));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


