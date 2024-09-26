---
title: ResourceAssignment.Guid
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment property. Gets or sets unique identifier for this assignment
type: docs
weight: 290
url: /net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

Gets or sets unique identifier for this assignment.

```csharp
public Guid? Guid { get; set; }
```

## Examples

Shows how to read an resource assignment GUID.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


