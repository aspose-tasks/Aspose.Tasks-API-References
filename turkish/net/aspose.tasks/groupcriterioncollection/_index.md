---
title: "Sınıf GroupCriterionCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.GroupCriterionCollection sınıfı. GroupCriterion nesnelerinin bir koleksiyonunu içerir. ICollectionGroupCriterion arayüzünü uygular."
type: docs
weight: 800
url: /tr/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

[`GroupCriterion`](../groupcriterion/) nesnelerinden oluşan bir koleksiyon içerir. ICollection&lt;GroupCriterion&gt; arayüzünü uygular.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Bir GroupCriterion koleksiyonunu [`GroupCriterion`](../groupcriterion/) nesnelerinden oluşan bir listeye dönüştürür. |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


