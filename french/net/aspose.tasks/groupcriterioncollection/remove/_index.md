---
title: "GroupCriterionCollection.Remove"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "méthode GroupCriterionCollection. Supprime la première occurrence d'un objet spécifique de cette collection"
type: docs
weight: 80
url: /fr/net/aspose.tasks/groupcriterioncollection/remove/
---
## GroupCriterionCollection.Remove method

Supprime la première occurrence d'un objet spécifique de cette collection.

```csharp
public bool Remove(GroupCriterion item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | GroupCriterion | l'objet spécifié à supprimer. |

### Valeur de retour

true si l'objet spécifié a été supprimé avec succès de cette collection ; sinon, false.

## Exemples

Montre comment travailler avec une collection de critères de groupe.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// itérer sur les critères de groupe
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

// copier les critères vers un autre groupe
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Voir aussi

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


