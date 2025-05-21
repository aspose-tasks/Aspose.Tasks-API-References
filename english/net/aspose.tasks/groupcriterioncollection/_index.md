---
title: Class GroupCriterionCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GroupCriterionCollection class. Contains a collection of GroupCriterion objects. Implements ICollectionGroupCriterion interface
type: docs
weight: 790
url: /net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Contains a collection of [`GroupCriterion`](../groupcriterion/) objects. Implements ICollection&lt;GroupCriterion&gt; interface.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Converts a GroupCriterion collection to a list of [`GroupCriterion`](../groupcriterion/) objects. |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


