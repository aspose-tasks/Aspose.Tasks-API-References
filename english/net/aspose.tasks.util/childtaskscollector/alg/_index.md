---
title: ChildTasksCollector.Alg
second_title: Aspose.Tasks for .NET API Reference
description: ChildTasksCollector method. Processes the specified object
type: docs
weight: 30
url: /net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Processes the specified object.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Type | Description |
| --- | --- | --- |
| el | Task | Object to process. |
| level | Int32 | Tree node level. |

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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


