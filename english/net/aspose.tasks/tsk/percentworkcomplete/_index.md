---
title: Tsk.PercentWorkComplete
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The current status of a task expressed as the percentage of work that has been completed
type: docs
weight: 890
url: /net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

The current status of a task expressed as the percentage of work that has been completed.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Examples

Shows how to read/write Tsk.PercentWorkComplete property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


