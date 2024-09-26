---
title: Tsk.RemainingDuration
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time that is required to complete the unfinished part of a task
type: docs
weight: 960
url: /net/aspose.tasks/tsk/remainingduration/
---
## Tsk.RemainingDuration field

The time that is required to complete the unfinished part of a task.

```csharp
public static readonly Key<Duration, TaskKey> RemainingDuration;
```

## Examples

Shows how to read/write Tsk.RemainingDuration property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Remaining Duration: " + task.Get(Tsk.RemainingDuration));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


