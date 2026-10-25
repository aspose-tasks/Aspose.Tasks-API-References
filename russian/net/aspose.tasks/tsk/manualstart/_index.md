---
title: "Tsk.ManualStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет вручную запланированный старт задачи"
type: docs
weight: 800
url: /ru/net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Определяет вручную запланированный старт задачи.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ManualStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


