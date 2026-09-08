---
title: "Tsk.PercentWorkComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Текущее состояние задачи, выраженное в процентах выполненной работы"
type: docs
weight: 890
url: /ru/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

Текущий статус задачи, выраженный в процентах выполненной работы.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


