---
title: AssignmentBaselineCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: AssignmentBaselineCollection method. Converts the AssignmentBaselineCollection object to a list of AssignmentBaseline objects
type: docs
weight: 70
url: /net/aspose.tasks/assignmentbaselinecollection/tolist/
---
## AssignmentBaselineCollection.ToList method

Converts the AssignmentBaselineCollection object to a list of [`AssignmentBaseline`](../../assignmentbaseline/) objects.

```csharp
public List<AssignmentBaseline> ToList()
```

### Return Value

List of [`AssignmentBaseline`](../../assignmentbaseline/) objects.

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


