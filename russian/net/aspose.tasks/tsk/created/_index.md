---
title: "Tsk.Created"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата создания задачи."
type: docs
weight: 250
url: /ru/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

Дата создания задачи.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Created.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


