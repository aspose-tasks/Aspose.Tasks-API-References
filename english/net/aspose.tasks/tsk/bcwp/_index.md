---
title: Tsk.BCWP
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The cumulative value of the tasks percent complete multiplied by the time phased baseline costs
type: docs
weight: 120
url: /net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

The cumulative value of the task's percent complete multiplied by the time phased baseline costs.

```csharp
public static readonly Key<double, TaskKey> BCWP;
```

## Examples

Shows how to read task cost values.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


