---
title: Project.GetPredecessors
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Returns a collection of task links which are predecessors of the specified task
type: docs
weight: 1120
url: /net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Returns a collection of task links which are predecessors of the specified task.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parameter | Type | Description |
| --- | --- | --- |
| task | Task | The task to get predecessors for. |

### Return Value

List of predecessors [`TaskLink`](../../tasklink/).

## Examples

Shows how to get predecessors for the specific task.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Display names of predecessor and successor tasks
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### See Also

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


