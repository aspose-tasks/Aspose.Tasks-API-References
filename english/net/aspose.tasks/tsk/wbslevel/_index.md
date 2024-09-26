---
title: Tsk.WBSLevel
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The rightmost WBS level of a task
type: docs
weight: 1140
url: /net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

The rightmost WBS level of a task.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Examples

Shows how to read task's WBS codes.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse through all the collected tasks
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


