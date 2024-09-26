---
title: Resource.Assignments
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets a collection of resource assignments for this object
type: docs
weight: 120
url: /net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

Gets a collection of resource assignments for this object.

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## Examples

Shows how to read assignments of a resource.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### See Also

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


