---
title: TaskBaselineCollection.Remove
second_title: Aspose.Tasks for .NET API Reference
description: TaskBaselineCollection method. Removes baseline from this collection
type: docs
weight: 50
url: /net/aspose.tasks/taskbaselinecollection/remove/
---
## TaskBaselineCollection.Remove method

Removes baseline from this collection.

```csharp
public bool Remove(TaskBaseline item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | TaskBaseline | The item to remove. |

### Return Value

true if the item has been removed successfully; otherwise, false

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


