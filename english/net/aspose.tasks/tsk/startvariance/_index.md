---
title: Tsk.StartVariance
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date
type: docs
weight: 1040
url: /net/aspose.tasks/tsk/startvariance/
---
## Tsk.StartVariance field

The time that represents the difference between a baseline start date of a task or assignment and its currently scheduled start date.

```csharp
public static readonly Key<Duration, TaskKey> StartVariance;
```

## Examples

Shows how to read/write Tsk.StartVariance property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartVariance, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Start Variance: " + task.Get(Tsk.StartVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


