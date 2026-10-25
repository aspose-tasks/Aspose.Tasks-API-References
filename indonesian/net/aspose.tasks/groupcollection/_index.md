---
title: "Kelas GroupCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.GroupCollection. Berisi daftar objek Group. Mengimplementasikan antarmuka ICollectionGroup."
type: docs
weight: 780
url: /id/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Berisi daftar objek [`Group`](../group/) . Mengimplementasikan antarmuka ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Mengonversi koleksi grup menjadi daftar objek [`Group`](../group/). |

## Contoh

Menampilkan cara bekerja dengan koleksi grup.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// iterasi grup tugas
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// iterasi grup sumber daya
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// hapus grup proyek lain
otherProject.TaskGroups.Clear();

// salin grup ke proyek lain
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// tambahkan grup tugas khusus
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// hapus semua grup
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Lihat Juga

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


