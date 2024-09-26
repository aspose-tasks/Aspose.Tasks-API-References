---
title: Tsk.ManualFinish
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Defines manually scheduled finish of a task
type: docs
weight: 790
url: /net/aspose.tasks/tsk/manualfinish/
---
## Tsk.ManualFinish field

Defines manually scheduled finish of a task.

```csharp
public static readonly Key<DateTime, TaskKey> ManualFinish;
```

## Examples

Shows how to read/write Tsk.ManualFinish property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Manual Finish: " + task.Get(Tsk.ManualFinish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


