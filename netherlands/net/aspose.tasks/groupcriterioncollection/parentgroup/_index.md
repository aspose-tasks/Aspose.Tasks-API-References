---
title: "GroupCriterionCollection.ParentGroup"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GroupCriterionCollection property. Haalt de ouder van het GroupCriterion-object op"
type: docs
weight: 30
url: /nl/net/aspose.tasks/groupcriterioncollection/parentgroup/
---
## GroupCriterionCollection.ParentGroup property

Haalt de ouder van het GroupCriterion-object op.

```csharp
public Group ParentGroup { get; }
```

## Voorbeelden

Toont hoe te werken met een collectie van groepscriteria.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// itereren over groepscriteria
Console.WriteLine("Print group criteria of {0} group: ", group.GroupCriteria.ParentGroup.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Index: " + criterion.Index);
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

// criteria kopiëren naar een andere groep
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Zie ook

* class [Group](../../group/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


