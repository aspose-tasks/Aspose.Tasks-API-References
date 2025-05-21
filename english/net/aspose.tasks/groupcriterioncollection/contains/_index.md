---
title: GroupCriterionCollection.Contains
second_title: Aspose.Tasks for .NET API Reference
description: GroupCriterionCollection method. Returns true if the specified item is found in this collection otherwise false
type: docs
weight: 50
url: /net/aspose.tasks/groupcriterioncollection/contains/
---
## GroupCriterionCollection.Contains method

Returns true if the specified item is found in this collection; otherwise, false.

```csharp
public bool Contains(GroupCriterion item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | GroupCriterion | the specified item to find. |

### Return Value

true if the specified item is found in this collection; otherwise, false.

## Examples

Shows how to work with a collection of group criterion.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// iterate over group criterion
Console.WriteLine("Print group criteria of the group '{0}': ", group.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Field: " + criterion.Field);
    Console.WriteLine("Group On: " + criterion.GroupOn);
    Console.WriteLine();
}

group.GroupCriteria.Clear();

if (!group.GroupCriteria.IsReadOnly)
{
    List<GroupCriterion> groupCriteria = group.GroupCriteria.ToList();
    foreach (var criterion in groupCriteria)
    {
        group.GroupCriteria.Remove(criterion);
    }
}

var criterionToAdd = new GroupCriterion
{
    Ascending = true,
    Field = Field.TaskActive
};

if (!group.GroupCriteria.Contains(criterionToAdd))
{
    group.GroupCriteria.Add(criterionToAdd);
}

// copy criteria to other group
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### See Also

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


