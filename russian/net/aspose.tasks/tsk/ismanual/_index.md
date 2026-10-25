---
title: "Tsk.IsManual"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача запланированной вручную"
type: docs
weight: 610
url: /ru/net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Определяет, запланирована ли задача вручную.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsManual.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


