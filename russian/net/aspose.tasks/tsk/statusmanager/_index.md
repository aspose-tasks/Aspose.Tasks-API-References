---
title: "Tsk.StatusManager"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Имя корпоративного ресурса, который будет получать обновления статуса текущей задачи от ресурсов"
type: docs
weight: 1050
url: /ru/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

Имя корпоративного ресурса, который будет получать обновления статуса текущей задачи от ресурсов.

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.StatusManager.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


