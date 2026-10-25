---
title: "GroupCriterionCollection.GetEnumerator"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "GroupCriterionCollection metodo. Restituisce un enumeratore per questa collezione"
type: docs
weight: 70
url: /it/net/aspose.tasks/groupcriterioncollection/getenumerator/
---
## GroupCriterionCollection.GetEnumerator method

Restituisce un enumeratore per questa collezione.

```csharp
public IEnumerator<GroupCriterion> GetEnumerator()
```

### Valore di ritorno

un enumeratore per questa collezione.

## Esempi

Mostra come lavorare con una raccolta di criteri di gruppo.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// itera sui criteri di gruppo
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

// copia i criteri in un altro gruppo
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Vedi anche

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


