---
title: "Tsk.LateStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Последняя дата, когда задача может начаться без задержки завершения проекта"
type: docs
weight: 740
url: /ru/net/aspose.tasks/tsk/latestart/
---
## Tsk.LateStart field

Последняя дата, к которой задача может начаться без задержки завершения проекта.

```csharp
public static readonly Key<DateTime, TaskKey> LateStart;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.LateStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LateStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Late Start: " + task.Get(Tsk.LateStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


