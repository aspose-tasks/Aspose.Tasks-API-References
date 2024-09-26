---
title: Tsk.IsRollup
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar
type: docs
weight: 690
url: /net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Determines whether information about the subtask Gantt bars will be rolled up to the summary task bar.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Examples

Shows how to read/write Tsk.IsRollup property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


