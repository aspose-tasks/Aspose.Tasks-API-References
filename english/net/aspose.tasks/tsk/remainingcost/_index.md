---
title: Tsk.RemainingCost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The remaining scheduled expense that will be incurred in completing the remaining scheduled work
type: docs
weight: 950
url: /net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

The remaining scheduled expense that will be incurred in completing the remaining scheduled work.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
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


