---
title: Tsk.ManualStart
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Defines manually scheduled start of a task
type: docs
weight: 800
url: /net/aspose.tasks/tsk/manualstart/
---
## Tsk.ManualStart field

Defines manually scheduled start of a task.

```csharp
public static readonly Key<DateTime, TaskKey> ManualStart;
```

## Examples

Shows how to read/write Tsk.ManualStart property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Start: " + task.Get(Tsk.ManualStart));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


