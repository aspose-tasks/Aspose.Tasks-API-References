---
title: Class TaskLink
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskLink class. Represents a predecessor link
type: docs
weight: 2370
url: /net/aspose.tasks/tasklink/
---
## TaskLink class

Represents a predecessor link.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Properties

| Name | Description |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Gets or sets the external predecessor project. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Gets or sets a value indicating whether a predecessor is part of another project. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Gets or sets the format for expressing the lag format. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Gets or sets the lag in tenths of a minute or percentage. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Gets or sets lag duration, depending on LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Gets or sets the type of a link. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Gets or sets the predecessor task. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Gets or sets the successor task. |

## Methods

| Name | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Returns a hash code value for the instance of the `TaskLink` class. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Returns string representation of a TaskLink. The exact details of the representation are unspecified and subject to change. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


