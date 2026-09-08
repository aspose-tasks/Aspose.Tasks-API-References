---
title: "Prj.TaskUpdatesResource"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, обновляются ли ресурсы при обновлении задач"
type: docs
weight: 710
url: /ru/net/aspose.tasks/prj/taskupdatesresource/
---
## Prj.TaskUpdatesResource field

Определяет, обновляют ли изменения задач ресурсы.

```csharp
public static readonly Key<NullableBool, PrjKey> TaskUpdatesResource;
```

## Примеры

Показывает, как читать/записывать свойство Prj.TaskUpdatesResource.

```csharp
var project = new Project();

project.Set(Prj.TaskUpdatesResource, true);

Console.WriteLine("Task Updates Resource: " + project.Get(Prj.TaskUpdatesResource));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


