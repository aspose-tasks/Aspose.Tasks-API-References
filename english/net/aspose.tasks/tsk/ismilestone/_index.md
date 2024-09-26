---
title: Tsk.IsMilestone
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is a milestone
type: docs
weight: 630
url: /net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

Determines whether a task is a milestone.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## Examples

Shows how to find estimated and/or milestone tasks.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Iterate over the collected tasks
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


