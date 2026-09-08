---
title: "Tsk.ManualFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет вручную запланированное завершение задачи"
type: docs
weight: 790
url: /ru/net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Определяет вручную запланированное завершение задачи.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.ManualFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


