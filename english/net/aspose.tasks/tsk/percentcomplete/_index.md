---
title: Tsk.PercentComplete
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The current status of a task expressed as the percentage of the tasks duration that has been completed
type: docs
weight: 880
url: /net/aspose.tasks/tsk/percentcomplete/
---
## Tsk.PercentComplete field

The current status of a task, expressed as the percentage of the task's duration that has been completed.

```csharp
public static readonly Key<int, TaskKey> PercentComplete;
```

## Examples

Shows how to change a task progress by updating of task percent complete.

```csharp
var project = new Project();
Console.WriteLine("Project Calculation mode is Automatic: {0}", project.CalculationMode.Equals(CalculationMode.Automatic));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(2));
task.Set(Tsk.PercentComplete, 50);

// Access tasks and display percentage completion
foreach (var tsk in project.RootTask.Children)
{
    Console.WriteLine(tsk.Get(Tsk.PercentComplete));
    Console.WriteLine(tsk.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(tsk.Get(Tsk.PhysicalPercentComplete));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


