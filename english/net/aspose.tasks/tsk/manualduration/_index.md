---
title: Tsk.ManualDuration
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Defines manually scheduled duration of a task
type: docs
weight: 780
url: /net/aspose.tasks/tsk/manualduration/
---
## Tsk.ManualDuration field

Defines manually scheduled duration of a task.

```csharp
public static readonly Key<Duration, TaskKey> ManualDuration;
```

## Examples

Shows how to read/write Tsk.ManualDuration property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ManualDuration, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Manual Duration: " + task.Get(Tsk.ManualDuration));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


