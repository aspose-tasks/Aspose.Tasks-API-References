---
title: Tsk.OutlineNumber
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The number that represents a tasks position in the hierarchical outline structure
type: docs
weight: 850
url: /net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

The number that represents a task's position in the hierarchical outline structure.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
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


