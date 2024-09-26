---
title: TaskBaselineCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaselineCollection property. Gets the number of objects contained in this TaskBaselineCollection object
type: docs
weight: 10
url: /net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Gets the number of objects contained in this TaskBaselineCollection object.

```csharp
public int Count { get; }
```

## Examples

Shows how to work with task baseline collections.

```csharp
var project = new Project();

// create project baselines
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// print task baselines
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// lets clear all baselines
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### See Also

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


