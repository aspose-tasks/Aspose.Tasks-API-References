---
title: "Tsk.ActualDuration"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Промежуток фактического рабочего времени задачи, основанный на запланированной длительности и текущей оставшейся работе или проценте выполнения"
type: docs
weight: 30
url: /ru/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

Период фактического рабочего времени задачи, основанный на запланированной длительности и текущей оставшейся работе или проценте выполнения.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## Примеры

Показывает, как читать фактические свойства задачи.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


