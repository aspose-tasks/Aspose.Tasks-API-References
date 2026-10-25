---
title: "Tsk.Guid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Сгенерированные уникальные идентификационные коды задачи"
type: docs
weight: 460
url: /ru/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

Сгенерированные уникальные коды идентификации задачи.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Guid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


