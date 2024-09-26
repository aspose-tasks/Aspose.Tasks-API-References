---
title: Tsk.PhysicalPercentComplete
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed BCWP
type: docs
weight: 900
url: /net/aspose.tasks/tsk/physicalpercentcomplete/
---
## Tsk.PhysicalPercentComplete field

Percent complete value that can be be used as an alternative for calculating budgeted cost of work performed (BCWP).

```csharp
public static readonly Key<int, TaskKey> PhysicalPercentComplete;
```

## Examples

Shows how to read/write Tsk.PhysicalPercentComplete property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PhysicalPercentComplete, 10);

Console.WriteLine("Physical Percent Complete: " + task.Get(Tsk.PhysicalPercentComplete));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


