---
title: "GroupCriterionCollection.Contains"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة GroupCriterionCollection. تُرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة وإلا false"
type: docs
weight: 50
url: /ar/net/aspose.tasks/groupcriterioncollection/contains/
---
## GroupCriterionCollection.Contains method

يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false.

```csharp
public bool Contains(GroupCriterion item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | GroupCriterion | العنصر المحدد للبحث عنه. |

### قيمة الإرجاع

صحيح إذا وُجد العنصر المحدد في هذه المجموعة؛ وإلا، خطأ.

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

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


