---
title: Class AssignmentBaselineCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.AssignmentBaselineCollection class. Represents a collection of AssignmentBaseline objects
type: docs
weight: 60
url: /net/aspose.tasks/assignmentbaselinecollection/
---
## AssignmentBaselineCollection class

Represents a collection of [`AssignmentBaseline`](../assignmentbaseline/) objects.

```csharp
public class AssignmentBaselineCollection : IList<AssignmentBaseline>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/assignmentbaselinecollection/count/) { get; } | Gets the number of objects contained in this AssignmentBaselineCollection object. |
| [Item](../../aspose.tasks/assignmentbaselinecollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentAssignment](../../aspose.tasks/assignmentbaselinecollection/parentassignment/) { get; } | Gets the parent [`ResourceAssignment`](../resourceassignment/) for this collection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/assignmentbaselinecollection/add/)(AssignmentBaseline) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [GetEnumerator](../../aspose.tasks/assignmentbaselinecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/assignmentbaselinecollection/remove/)(AssignmentBaseline) | Removes baseline from this collection. |
| [ToList](../../aspose.tasks/assignmentbaselinecollection/tolist/)() | Converts the AssignmentBaselineCollection object to a list of [`AssignmentBaseline`](../assignmentbaseline/) objects. |

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

* class [AssignmentBaseline](../assignmentbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


