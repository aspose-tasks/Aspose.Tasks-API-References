---
title: Tsk.RemainingOvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The remaining scheduled overtime expense for a task
type: docs
weight: 970
url: /net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

The remaining scheduled overtime expense for a task.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Examples

Shows how to read/write Tsk.RemainingOvertimeCost property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


