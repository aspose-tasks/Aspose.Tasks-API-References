---
title: Task.Assignments
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets a collection of resource assignments for this object
type: docs
weight: 120
url: /net/aspose.tasks/task/assignments/
---
## Task.Assignments property

Gets a collection of resource assignments for this object.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Examples

Shows how to iterate over task's assignments.

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

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


