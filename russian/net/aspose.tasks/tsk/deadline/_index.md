---
title: "Tsk.Deadline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Целевая дата, указывающая, когда задача должна быть завершена"
type: docs
weight: 270
url: /ru/net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

Целевая дата, указывающая, когда задача должна быть завершена.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.Deadline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


