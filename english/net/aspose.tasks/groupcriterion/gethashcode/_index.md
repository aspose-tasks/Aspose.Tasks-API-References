---
title: GroupCriterion.GetHashCode
second_title: Aspose.Tasks for .NET API Reference
description: GroupCriterion method. Serves as a hash function for a particular type
type: docs
weight: 140
url: /net/aspose.tasks/groupcriterion/gethashcode/
---
## GroupCriterion.GetHashCode method

Serves as a hash function for a particular type.

```csharp
public override int GetHashCode()
```

### Return Value

A hash code for the current Object.

## Examples

Shows how to use hash code of a group criterion.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");
var group = project.TaskGroups.ToList()[1];

// get the first group criteria
var criterion = group.GroupCriteria.ToList()[0];

// each GroupCriterion has internal GUID which hash code is based on
Console.WriteLine("Task Criterion HashCode: " + criterion.GetHashCode());

// work with group criteria...
```

### See Also

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


