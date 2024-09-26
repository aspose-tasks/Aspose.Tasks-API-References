---
title: Tsk.OutlineLevel
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The outline level of a task
type: docs
weight: 840
url: /net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

The outline level of a task.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## Examples

Shows how to read task outline properties.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


