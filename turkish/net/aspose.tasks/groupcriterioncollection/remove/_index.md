---
title: "GroupCriterionCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GroupCriterionCollection metodu. Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır"
type: docs
weight: 80
url: /tr/net/aspose.tasks/groupcriterioncollection/remove/
---
## GroupCriterionCollection.Remove method

Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır.

```csharp
public bool Remove(GroupCriterion item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | GroupCriterion | kaldırılacak belirtilen nesne. |

### Dönüş Değeri

Bu koleksiyondan belirtilen nesne başarıyla kaldırıldıysa doğru; aksi takdirde yanlış.

## Örnekler

Bir grup kriter koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// grup kriterleri üzerinde yineleme yap
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

// kriterleri başka bir gruba kopyala
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Ayrıca Bakınız

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


