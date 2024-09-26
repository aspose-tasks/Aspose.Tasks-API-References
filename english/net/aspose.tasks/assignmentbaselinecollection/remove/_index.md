---
title: AssignmentBaselineCollection.Remove
second_title: Aspose.Tasks for .NET API Reference
description: AssignmentBaselineCollection method. Removes baseline from this collection
type: docs
weight: 60
url: /net/aspose.tasks/assignmentbaselinecollection/remove/
---
## AssignmentBaselineCollection.Remove method

Removes baseline from this collection.

```csharp
public bool Remove(AssignmentBaseline item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | AssignmentBaseline | The item to remove. |

### Return Value

true if [`AssignmentBaseline`](../../assignmentbaseline/) instance has been removed successfully; otherwise, false

## Examples

Shows how to read assignment baselines.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// read assignment baseline information
foreach (var assignment in project.ResourceAssignments)
{
    var baselines = assignment.Baselines;
    Console.WriteLine("Count of assignment baselines: " + baselines.Count);
    Console.WriteLine("Parent Assignment: " + baselines.ParentAssignment);
    foreach (var baseline in baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
    }

    Console.WriteLine();
}

Console.WriteLine("Delete all assignment baselines: ");

// delete assignment baselines
foreach (var assignment in project.ResourceAssignments)
{
    List<AssignmentBaseline> baselines = assignment.Baselines.ToList();
    foreach (var baseline in baselines)
    {
        assignment.Baselines.Remove(baseline);
    }
}
```

### See Also

* class [AssignmentBaseline](../../assignmentbaseline/)
* class [AssignmentBaselineCollection](../)
* namespace [Aspose.Tasks](../../assignmentbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


