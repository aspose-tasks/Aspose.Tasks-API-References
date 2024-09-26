---
title: ResourceAssignment.ParentProject
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment property. Gets parent project for this assignment
type: docs
weight: 420
url: /net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

Gets parent project for this assignment.

```csharp
public Project ParentProject { get; }
```

## Examples

Shows how to use parent project of a resource assignment.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// set a duration of the assignment by using default project time unit type.
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### See Also

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


