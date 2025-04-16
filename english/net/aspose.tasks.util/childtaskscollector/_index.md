---
title: Class ChildTasksCollector
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Util.ChildTasksCollector class. Collects all child tasks
type: docs
weight: 2610
url: /net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Collects all child tasks.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Constructors

| Name | Description |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Initializes a new instance of the `ChildTasksCollector` class. |

## Properties

| Name | Description |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Gets a list collected child objects (tasks). |

## Methods

| Name | Description |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Processes the specified object. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Examples

Shows how to iterate over all tasks in a project as a plain list.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### See Also

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


