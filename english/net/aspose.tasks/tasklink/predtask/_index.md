---
title: TaskLink.PredTask
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink property. Gets or sets the predecessor task
type: docs
weight: 70
url: /net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Gets or sets the predecessor task.

```csharp
public Task PredTask { get; set; }
```

## Examples

Shows how to read project task links.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Display names of predecessor and successor tasks
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### See Also

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


