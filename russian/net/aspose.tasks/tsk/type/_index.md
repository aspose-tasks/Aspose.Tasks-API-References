---
title: "Tsk.Type"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Тип задачи."
type: docs
weight: 1100
url: /ru/net/aspose.tasks/tsk/type/
---
## Tsk.Type field

Тип задачи.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Type.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


