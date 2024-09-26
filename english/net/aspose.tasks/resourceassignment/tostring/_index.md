---
title: ResourceAssignment.ToString
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Returns short string representation of the instance of the ResourceAssignment class. The exact details of the representation are unspecified and subject to change
type: docs
weight: 790
url: /net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

Returns short string representation of the instance of the [`ResourceAssignment`](../) class. The exact details of the representation are unspecified and subject to change.

```csharp
public override string ToString()
```

### Return Value

short string which represents assignment object.

## Examples

Shows how to print common assignment info.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // display task's assignments
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


