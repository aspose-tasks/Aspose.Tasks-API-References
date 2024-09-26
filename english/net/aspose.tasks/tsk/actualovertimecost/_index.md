---
title: Tsk.ActualOvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Costs incurred for overtime work already performed on tasks by assigned resources
type: docs
weight: 50
url: /net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Costs incurred for overtime work already performed on tasks by assigned resources.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Examples

Shows how to read/write Tsk.ActualOvertimeCost property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


