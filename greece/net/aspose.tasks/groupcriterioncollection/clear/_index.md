---
title: "GroupCriterionCollection.Clear"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GroupCriterionCollection μέθοδος. Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή"
type: docs
weight: 40
url: /el/net/aspose.tasks/groupcriterioncollection/clear/
---
## GroupCriterionCollection.Clear method

Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή.

```csharp
public void Clear()
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με μια συλλογή κριτηρίων ομάδας.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// επανάληψη πάνω από κριτήρια ομάδας
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

// αντιγραφή κριτηρίων σε άλλη ομάδα
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Δείτε επίσης

* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


