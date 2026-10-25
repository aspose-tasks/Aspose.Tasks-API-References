---
title: "Tsk.IsRollup"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, будет ли информация о гантовых столбцах подпроекта свёрнута в столбец сводной задачи"
type: docs
weight: 690
url: /ru/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Определяет, будет ли информация о полосах Ганта подзадач агрегирована в полосу сводной задачи.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsRollup.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


