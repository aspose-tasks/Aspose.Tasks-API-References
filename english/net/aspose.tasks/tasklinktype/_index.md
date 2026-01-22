---
title: Enum TaskLinkType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.TaskLinkType enum. Specifies the type of tasks dependency
type: docs
weight: 2410
url: /net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

Specifies the type of tasks dependency.

```csharp
public enum TaskLinkType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| FinishToFinish | `0` | Finish-Finish relationship |
| FinishToStart | `1` | Finish-Start relationship |
| StartToFinish | `2` | Start-Finish relationship |
| StartToStart | `3` | Start-Start relationship |

## Examples

Shows how to get/set a link type of a task link.

```csharp
var project = new Project();

// Add new tasks
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Link tasks with link type set to Start to Start
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


