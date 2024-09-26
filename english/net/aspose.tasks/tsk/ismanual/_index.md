---
title: Tsk.IsManual
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is manually scheduled
type: docs
weight: 610
url: /net/aspose.tasks/tsk/ismanual/
---
## Tsk.IsManual field

Determines whether a task is manually scheduled.

```csharp
public static readonly Key<NullableBool, TaskKey> IsManual;
```

## Examples

Shows how to read/write Tsk.IsManual property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsManual, true);

Console.WriteLine("Is Manual: " + task.Get(Tsk.IsManual));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


