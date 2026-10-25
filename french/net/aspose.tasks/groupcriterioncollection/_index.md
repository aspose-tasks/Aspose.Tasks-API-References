---
title: "Classe GroupCriterionCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.GroupCriterionCollection. Contient une collection d’objets GroupCriterion. Implémente l’interface ICollectionGroupCriterion."
type: docs
weight: 800
url: /fr/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Contient une collection d'objets [`GroupCriterion`](../groupcriterion/). Implémente l'interface ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Convertit une collection GroupCriterion en une liste d'objets [`GroupCriterion`](../groupcriterion/). |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


