---
title: "Tsk.ActualCost"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Затраты, понесённые за уже выполненную работу ресурсами по их задачам, а также любые другие зарегистрированные затраты, связанные с задачей"
type: docs
weight: 20
url: /ru/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Затраты, понесённые за работу, уже выполненную ресурсами по их задачам, вместе с любыми другими зарегистрированными затратами, связанными с задачей.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


