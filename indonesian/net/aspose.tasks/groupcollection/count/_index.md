---
title: "GroupCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GroupCollection. Mendapatkan jumlah elemen yang terdapat dalam koleksi ini."
type: docs
weight: 10
url: /id/net/aspose.tasks/groupcollection/count/
---
## GroupCollection.Count property

Mendapatkan jumlah elemen yang terdapat dalam koleksi ini.

```csharp
public int Count { get; }
```

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

* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


