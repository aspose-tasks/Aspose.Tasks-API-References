---
title: "GroupCriterionCollection.IsReadOnly"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية GroupCriterionCollection. يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط وإلا false"
type: docs
weight: 20
url: /ar/net/aspose.tasks/groupcriterioncollection/isreadonly/
---
## GroupCriterionCollection.IsReadOnly property

يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false.

```csharp
public bool IsReadOnly { get; }
```

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

* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


