---
title: Project.TaskLinks
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets TaskLinkCollection object
type: docs
weight: 930
url: /net/aspose.tasks/project/tasklinks/
---
## Project.TaskLinks property

Gets [`TaskLinkCollection`](../../tasklinkcollection/) object.

```csharp
public TaskLinkCollection TaskLinks { get; }
```

## Examples

Shows how to create task links.

```csharp
var project = new Project();

// Add new tasks
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// Link tasks
project.TaskLinks.Add(pred, succ);

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Predecessor Task: " + link.PredTask);
    Console.WriteLine("Successor Task: " + link.SuccTask);
    Console.WriteLine("LagFormat: " + link.LagFormat);
    Console.WriteLine("LinkType: " + link.LinkType);
    Console.WriteLine("LinkLag: " + link.LinkLag);
    Console.WriteLine("CrossProjectName: " + link.CrossProjectName);
    Console.WriteLine("IsCrossProject: " + link.IsCrossProject);
}
```

### See Also

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


