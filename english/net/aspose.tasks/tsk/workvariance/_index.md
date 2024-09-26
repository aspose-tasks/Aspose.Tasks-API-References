---
title: Tsk.WorkVariance
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The difference between baseline work of a task and the currently scheduled work
type: docs
weight: 1160
url: /net/aspose.tasks/tsk/workvariance/
---
## Tsk.WorkVariance field

The difference between baseline work of a task and the currently scheduled work.

```csharp
public static readonly Key<Duration, TaskKey> WorkVariance;
```

## Examples

Shows how to read/write Tsk.WorkVariance property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.WorkVariance, project.GetDuration(1));

Console.WriteLine("Work Variance: " + task.Get(Tsk.WorkVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


