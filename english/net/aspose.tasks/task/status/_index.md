---
title: Task.Status
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets task status
type: docs
weight: 1160
url: /net/aspose.tasks/task/status/
---
## Task.Status property

Gets task status.

```csharp
public TaskStatus Status { get; }
```

## Examples

Shows how to get task's status.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Project's status date should be set because status calculation uses status date.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### See Also

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


