---
title: Task.Baselines
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets or sets the collection of baseline values of the task
type: docs
weight: 130
url: /net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Gets or sets the collection of baseline values of the task.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Examples

Shows how to read task's baselines.

```csharp
var project = new Project();

// set a baseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Display task baseline duration
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### See Also

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


