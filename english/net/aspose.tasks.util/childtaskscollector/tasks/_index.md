---
title: ChildTasksCollector.Tasks
second_title: Aspose.Tasks for .NET API Reference
description: ChildTasksCollector property. Gets a list collected child objects tasks
type: docs
weight: 20
url: /net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Gets a list collected child objects (tasks).

```csharp
public List<Task> Tasks { get; }
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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


