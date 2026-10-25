---
title: "GroupCriterionCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GroupCriterionCollection methode. Verwijdert de eerste voorkoming van een specifiek object uit deze collectie"
type: docs
weight: 80
url: /nl/net/aspose.tasks/groupcriterioncollection/remove/
---
## GroupCriterionCollection.Remove method

Verwijdert de eerste instantie van een specifiek object uit deze collectie.

```csharp
public bool Remove(GroupCriterion item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | GroupCriterion | het opgegeven object om te verwijderen. |

### Retourwaarde

true als het opgegeven object succesvol uit deze collectie is verwijderd; anders false.

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


