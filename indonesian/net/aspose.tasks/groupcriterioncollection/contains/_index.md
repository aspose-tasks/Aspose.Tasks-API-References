---
title: "GroupCriterionCollection.Contains"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "metode GroupCriterionCollection. Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini, jika tidak false."
type: docs
weight: 50
url: /id/net/aspose.tasks/groupcriterioncollection/contains/
---
## GroupCriterionCollection.Contains method

Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.

```csharp
public bool Contains(GroupCriterion item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | GroupCriterion | item yang ditentukan untuk dicari. |

### Nilai Kembali

true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.

## Contoh

Menampilkan cara bekerja dengan koleksi kriteria grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

var group = project.TaskGroups.ToList()[0];

// iterasi atas kriteria grup
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

* class [GroupCriterion](../../groupcriterion/)
* class [GroupCriterionCollection](../)
* namespace [Aspose.Tasks](../../groupcriterioncollection/)
* assembly [Aspose.Tasks](../../../)


