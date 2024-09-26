---
title: Tsk.IsCritical
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is on the critical path
type: docs
weight: 560
url: /net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Determines whether a task is on the critical path.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Examples

Shows how to find critical and/or effort driven tasks.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


