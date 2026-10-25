---
title: "Kelas GroupCriterionCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.GroupCriterionCollection. Berisi koleksi objek GroupCriterion. Mengimplementasikan antarmuka ICollectionGroupCriterion."
type: docs
weight: 800
url: /id/net/aspose.tasks/groupcriterioncollection/
---
## GroupCriterionCollection class

Berisi koleksi objek [`GroupCriterion`](../groupcriterion/). Mengimplementasikan antarmuka ICollection&lt;GroupCriterion&gt;.

```csharp
public class GroupCriterionCollection : IList<GroupCriterion>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/groupcriterioncollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/groupcriterioncollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/groupcriterioncollection/add/)(GroupCriterion) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/groupcriterioncollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/groupcriterioncollection/contains/)(GroupCriterion) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/groupcriterioncollection/copyto/)(GroupCriterion[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/groupcriterioncollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/groupcriterioncollection/remove/)(GroupCriterion) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [ToList](../../aspose.tasks/groupcriterioncollection/tolist/)() | Mengonversi koleksi GroupCriterion menjadi daftar objek [`GroupCriterion`](../groupcriterion/). |

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

* class [GroupCriterion](../groupcriterion/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


