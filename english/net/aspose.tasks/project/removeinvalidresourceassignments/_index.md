---
title: Project.RemoveInvalidResourceAssignments
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Eliminates invalid resource assignments from the project resource assignments list
type: docs
weight: 1180
url: /net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Eliminates invalid resource assignments from the project resource assignments list.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Remarks

MS Project creates an empty resource assignment for each task. Call the method to remove them.

## Examples

Shows how to remove invalid assignments.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// remove invalid assignments
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


