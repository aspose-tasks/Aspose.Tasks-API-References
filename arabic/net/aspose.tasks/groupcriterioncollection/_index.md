---
title: "الفئة GroupCriterionCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.GroupCriterionCollection. تحتوي على مجموعة من كائنات GroupCriterion. تنفذ واجهة ICollectionGroupCriterion."
type: docs
weight: 800
url: /ar/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

تحتوي على مجموعة من [`GroupCriterion`](../groupcriterion/) كائنات. تنفذ واجهة ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | تحول مجموعة GroupCriterion إلى قائمة من كائنات [`GroupCriterion`](../groupcriterion/). |

## الأمثلة

يوضح كيفية العمل مع مجموعة من معايير المجموعة.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// تكرار عبر معايير المجموعة
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

// نسخ المعايير إلى مجموعة أخرى
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### انظر أيضًا

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


