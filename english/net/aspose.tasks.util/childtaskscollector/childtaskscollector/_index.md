---
title: ChildTasksCollector.ChildTasksCollector
second_title: Aspose.Tasks for .NET API Reference
description: ChildTasksCollector constructor. Initializes a new instance of the ChildTasksCollector class
type: docs
weight: 10
url: /net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Initializes a new instance of the [`ChildTasksCollector`](../) class.

```csharp
public ChildTasksCollector()
```

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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


