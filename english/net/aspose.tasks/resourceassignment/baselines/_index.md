---
title: ResourceAssignment.Baselines
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment property. Gets AssignmentBaselineCollection object. The collection of baseline values associated with an assignment
type: docs
weight: 120
url: /net/aspose.tasks/resourceassignment/baselines/
---
## ResourceAssignment.Baselines property

Gets AssignmentBaselineCollection object. The collection of baseline values associated with an assignment.

```csharp
public AssignmentBaselineCollection Baselines { get; }
```

## Examples

Shows how to get access to assignment's baselines.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

project.SetBaseline(BaselineType.Baseline);

foreach (var assignmentBaseline in resourceAssignment.Baselines)
{
    Console.WriteLine("Baseline Start: {0}", assignmentBaseline.Start);
    Console.WriteLine("Baseline Finish: {0}", assignmentBaseline.Finish);
}
```

### See Also

* class [AssignmentBaselineCollection](../../assignmentbaselinecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


