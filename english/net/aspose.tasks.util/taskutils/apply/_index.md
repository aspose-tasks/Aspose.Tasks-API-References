---
title: TaskUtils.Apply
second_title: Aspose.Tasks for .NET API Reference
description: TaskUtils method. Applies specified algorithm to each task of a tree
type: docs
weight: 10
url: /net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Applies specified algorithm to each task of a tree.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| root | Task | Root of the tree |
| alg | ITreeAlgorithm`1 | Applied algorithm. |
| level | Int32 | Level of the root task. |

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

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


