---
title: Tsk.ActualDuration
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The span of actual working time for a task based on the scheduled duration and current remaining work or percent complete
type: docs
weight: 30
url: /net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

The span of actual working time for a task, based on the scheduled duration and current remaining work or percent complete.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


