---
title: Tsk.ActualCost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Costs incurred for work already performed by resources on their tasks together with any other recorded costs associated with the task
type: docs
weight: 20
url: /net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Costs incurred for work already performed by resources on their tasks, together with any other recorded costs associated with the task.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Examples

Shows how to read task's actual properties.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


