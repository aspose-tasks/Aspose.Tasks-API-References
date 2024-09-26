---
title: Tsk.FinishVariance
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time that represents the difference between the baseline finish date of a task or assignment and its current finish date
type: docs
weight: 420
url: /net/aspose.tasks/tsk/finishvariance/
---
## Tsk.FinishVariance field

The time that represents the difference between the baseline finish date of a task or assignment and its current finish date.

```csharp
public static readonly Key<Duration, TaskKey> FinishVariance;
```

## Examples

Shows how to read/write Tsk.FinishVariance property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Finish Variance: " + task.Get(Tsk.FinishVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


