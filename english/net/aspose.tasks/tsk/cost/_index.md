---
title: Tsk.Cost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks in addition to the costs planned for the remaining work
type: docs
weight: 230
url: /net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

The total scheduled or projected cost for a task based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work.

```csharp
public static readonly Key<decimal, TaskKey> Cost;
```

## Examples

Shows how to read task costs.

```csharp
var project = new Project();

// Add task and set cost
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Display cost related properties of task
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


