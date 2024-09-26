---
title: TaskLink.LinkType
second_title: Aspose.Tasks for .NET API Reference
description: TaskLink property. Gets or sets the type of a link
type: docs
weight: 60
url: /net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

Gets or sets the type of a link.

```csharp
public TaskLinkType LinkType { get; set; }
```

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

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


