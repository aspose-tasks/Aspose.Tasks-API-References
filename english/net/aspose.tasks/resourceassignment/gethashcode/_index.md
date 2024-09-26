---
title: ResourceAssignment.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Returns a hash code value for the instance of the ResourceAssignment class
type: docs
weight: 710
url: /net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Returns a hash code value for the instance of the [`ResourceAssignment`](../) class.

```csharp
public override int GetHashCode()
```

### Return Value

returns a hash code value for this object.

## Examples

Shows how to get a hash code of a resource assignment.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// print assignment's hash codes
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### See Also

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


