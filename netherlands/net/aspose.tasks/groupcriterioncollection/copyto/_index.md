---
title: "GroupCriterionCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GroupCriterionCollection methode. Kopieert de elementen van deze collectie naar de opgegeven array beginnend bij de opgegeven array-index"
type: docs
weight: 60
url: /nl/net/aspose.tasks/groupcriterioncollection/copyto/
---
## GroupCriterionCollection.CopyTo method

Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index.

```csharp
public void CopyTo(GroupCriterion[] array, int arrayIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | GroupCriterion[] | de opgegeven eendimensionale array om elementen naartoe te kopiëren |
| arrayIndex | Int32 | de nulgebaseerde index van de opgegeven array waarop het kopiëren begint. |

## Voorbeelden

Toont hoe te werken met een collectie van groepscriteria.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// itereren over groepscriteria
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

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


