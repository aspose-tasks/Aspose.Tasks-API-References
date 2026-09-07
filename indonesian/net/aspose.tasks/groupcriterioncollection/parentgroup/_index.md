---
title: "GroupCriterionCollection.ParentGroup"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GroupCriterionCollection. Mendapatkan induk dari objek GroupCriterion"
type: docs
weight: 30
url: /id/net/aspose.tasks/groupcriterioncollection/parentgroup/
---
## GroupCriterionCollection.ParentGroup property

Mendapatkan induk dari objek GroupCriterion.

```csharp
public Group ParentGroup { get; }
```

## Contoh

Menampilkan cara bekerja dengan koleksi kriteria grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// iterasi atas kriteria grup
Console.WriteLine("Print group criteria of {0} group: ", group.GroupCriteria.ParentGroup.Name);
Console.WriteLine("Group criterion count: " + group.GroupCriteria.Count);
foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Index: " + criterion.Index);
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

// salin kriteria ke grup lain
var otherGroup = project.TaskGroups.ToList()[0];

var criteria = new GroupCriterion[group.GroupCriteria.Count];
group.GroupCriteria.CopyTo(criteria, 0);
foreach (var criterion in criteria)
{
    otherGroup.GroupCriteria.Add(criterion);
}
```

### Lihat Juga

* class [Group](../../group/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


