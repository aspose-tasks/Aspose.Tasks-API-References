---
title: Tsk.OvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The amount of overtime scheduled to be performed by all resources assigned to a task
type: docs
weight: 870
url: /net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

The amount of overtime scheduled to be performed by all resources assigned to a task.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


