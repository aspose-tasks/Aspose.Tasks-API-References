---
title: "Tsk.StartVariance"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Время, представляющее разницу между базовой датой начала задачи или назначения и её текущей запланированной датой начала"
type: docs
weight: 1040
url: /ru/net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

Время, представляющее разницу между базовой датой начала задачи или назначения и её текущей запланированной датой начала.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.StartVariance.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


