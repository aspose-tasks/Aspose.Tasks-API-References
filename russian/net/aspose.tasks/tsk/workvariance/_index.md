---
title: "Tsk.WorkVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Разница между базовой работой задачи и текущей запланированной работой"
type: docs
weight: 1160
url: /ru/net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

Разница между базовой работой задачи и текущей запланированной работой.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.WorkVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


