---
title: Tsk.CostVariance
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The difference between the baseline cost and total cost for a task resource or assignment
type: docs
weight: 240
url: /net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

The difference between the baseline cost and total cost for a task, resource, or assignment.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


