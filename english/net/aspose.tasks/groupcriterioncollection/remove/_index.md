---
title: GroupCriterionCollection.Remove
second_title: Aspose.Tasks for .NET API Reference
description: GroupCriterionCollection method. Removes the first occurrence of a specific object from this collection
type: docs
weight: 80
url: /net/aspose.tasks/groupcriterioncollection/remove/
---
## GroupCriterionCollection.Remove method

Removes the first occurrence of a specific object from this collection.

```csharp
public bool Remove(GroupCriterion item)
```

| Parameter | Type | Description |
| --- | --- | --- |
| item | GroupCriterion | the specified object to remove. |

### Return Value

true if the specified object was successfully removed from this collection; otherwise, false.

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


