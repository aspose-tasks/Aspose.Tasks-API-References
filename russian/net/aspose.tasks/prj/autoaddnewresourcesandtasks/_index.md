---
title: "Prj.AutoAddNewResourcesAndTasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Определяет, добавляются ли новые ресурсы или задачи автоматически в пул ресурсов или задач"
type: docs
weight: 50
url: /ru/net/aspose.tasks/prj/autoaddnewresourcesandtasks/
---
## Prj.AutoAddNewResourcesAndTasks field

Определяет, добавляются ли новые ресурсы или задачи автоматически в пул ресурсов или задач.

```csharp
public static readonly Key<NullableBool, PrjKey> AutoAddNewResourcesAndTasks;
```

## Примеры

Показывает, как читать/записывать свойство Prj.AutoAddNewResourcesAndTasks.

```csharp
var project = new Project();

project.Set(Prj.AutoAddNewResourcesAndTasks, true);

Console.WriteLine("Auto Add New Resources And Tasks: " + project.Get(Prj.AutoAddNewResourcesAndTasks));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


