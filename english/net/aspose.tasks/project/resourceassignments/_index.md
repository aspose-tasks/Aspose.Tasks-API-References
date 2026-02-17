---
title: Project.ResourceAssignments
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets ResourceAssignmentCollection object
type: docs
weight: 750
url: /net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

Gets ResourceAssignmentCollection object.

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## Examples

Shows how to work with resource assignments.

```csharp
var project = new Project();

// Add new task and resource
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// Assign the resource desired task
project.ResourceAssignments.Add(task, resource);
```

### See Also

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


