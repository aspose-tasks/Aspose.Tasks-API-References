---
title: Tsk.DurationVariance
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The difference between the baseline duration of a task and the total duration current estimate of a task
type: docs
weight: 320
url: /net/aspose.tasks/tsk/durationvariance/
---
## Tsk.DurationVariance field

The difference between the baseline duration of a task and the total duration (current estimate) of a task.

```csharp
public static readonly Key<Duration, TaskKey> DurationVariance;
```

## Examples

Shows how to read/write Tsk.DurationVariance property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationVariance, project.GetWork(1));

Console.WriteLine("Duration Variance: " + task.Get(Tsk.DurationVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


