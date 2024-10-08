---
title: GroupCriterion.Equals
second_title: Aspose.Tasks for .NET API Reference
description: GroupCriterion method. Returns a value indicating whether this instance is equal to a specified object
type: docs
weight: 130
url: /net/aspose.tasks/groupcriterion/equals/
---
## GroupCriterion.Equals method

Returns a value indicating whether this instance is equal to a specified object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object to compare with this instance. |

### Return Value

**True** if o is a GroupCriterion that has the same UID value as this instance; otherwise, **false**.

## Examples

Shows how to check equality of group criteria.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");
var group = project.TaskGroups.ToList()[1];

// get the first group criteria
List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
var criterion1 = groupCriteria[0];
var criterion2 = groupCriteria[0];

// group criteria equality is based on public member 'Field'  
Console.WriteLine("Task Criterion 1 Field: " + criterion1.Field);
Console.WriteLine("Task Criterion 2 Field: " + criterion2.Field);
Console.WriteLine("Are the criteria equal: " + criterion1.Equals(criterion2));
```

### See Also

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)


