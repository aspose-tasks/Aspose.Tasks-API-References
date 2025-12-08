---
title: Class TaskBaselineCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskBaselineCollection class. Represents a collection of TaskBaseline objects
type: docs
weight: 2340
url: /net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Represents a collection of [`TaskBaseline`](../taskbaseline/) objects.

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Gets the number of objects contained in this TaskBaselineCollection object. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Returns the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Removes baseline from this collection. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Converts the TaskBaselineCollection object to a list of [`TaskBaseline`](../taskbaseline/) objects. |

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

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


