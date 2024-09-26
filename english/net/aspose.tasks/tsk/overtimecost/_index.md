---
title: Tsk.OvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The total overtime cost for a task for a resource on all assigned tasks or for a resource assignment
type: docs
weight: 860
url: /net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

The total overtime cost for a task, for a resource on all assigned tasks, or for a resource assignment.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
```

## Examples

Shows how to read task overtimes.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Read overtime and percentage completion for tasks
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Set percent complete
    task.Set(Tsk.PercentComplete, 100);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


