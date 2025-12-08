---
title: Class TaskUtils
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.TaskUtils class. Helper class which provides useful operations with tasks
type: docs
weight: 2720
url: /net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Helper class which provides useful operations with tasks.

```csharp
public static class TaskUtils
```

## Methods

| Name | Description |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Applies specified algorithm to each task of a tree. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Builds new tree of tasks which satisfy the condition. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Finds a task which satisfy the condition in a tree of tasks. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Recursively calculates a number of task's children tasks through all levels. |

## Examples

Shows how to work with a tree algorithm.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// gather all project tasks
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// work with tasks as with a plain list
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### See Also

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


