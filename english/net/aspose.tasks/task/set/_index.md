---
title: Task.Set
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Maps the specified property to the specified value in this container
type: docs
weight: 1410
url: /net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Maps the specified property to the specified value in this container.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Parameter | Description |
| --- | --- |
| T | the type of the mapped value. |
| key | the specified property key. [`Tsk`](../../tsk/) for getting the property key. |
| val | the value. |

## Examples

Shows how to get/set task properties.

```csharp
var project = new Project();

// Add task and set task properties
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


