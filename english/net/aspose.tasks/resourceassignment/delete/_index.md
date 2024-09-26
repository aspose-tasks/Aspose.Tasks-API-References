---
title: ResourceAssignment.Delete
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Deletes resource assignment from project assignments collection
type: docs
weight: 680
url: /net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

Deletes resource assignment from project assignments collection.

```csharp
public void Delete()
```

## Examples

Shows how to delete a resource assignment.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


