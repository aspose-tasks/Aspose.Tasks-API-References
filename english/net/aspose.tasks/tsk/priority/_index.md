---
title: Tsk.Priority
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The level of importance given to a task which in turn indicates how readily a task or assignment can be delayed or split during resource leveling
type: docs
weight: 930
url: /net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

The level of importance given to a task, which in turn indicates how readily a task or assignment can be delayed or split during resource leveling.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Examples

Shows how to read a task priority.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Display Priorities for all tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


