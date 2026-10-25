---
title: "Klasse GroupCriterionCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.GroupCriterionCollection‑klasse. Bevat een collectie van GroupCriterion‑objecten. Implementeert de ICollectionGroupCriterion‑interface."
type: docs
weight: 800
url: /nl/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Bevat een collectie van [`GroupCriterion`](../groupcriterion/) objecten. Implementeert de ICollection&lt;GroupCriterion&gt; interface.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Converteert een GroupCriterion-collectie naar een lijst van [`GroupCriterion`](../groupcriterion/) objecten. |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


