---
title: TaskLink.LagFormat
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink property. Gets or sets the format for expressing the lag format
type: docs
weight: 30
url: /net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Gets or sets the format for expressing the lag format.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


