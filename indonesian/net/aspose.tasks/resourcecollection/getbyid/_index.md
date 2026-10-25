---
title: "ResourceCollection.GetById"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceCollection. Mengembalikan sumber daya dengan id yang ditentukan"
type: docs
weight: 60
url: /id/net/aspose.tasks/resourcecollection/getbyid/
---
## ResourceCollection.GetById method

Mengembalikan sumber daya dengan id yang ditentukan.

```csharp
public Resource GetById(int id)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| id | Int32 | Id yang ditentukan. |

### Nilai Kembali

Sumber daya dengan id yang ditentukan jika ada; jika tidak, null.

## Catatan

Kompleksitas O(1).

## Contoh

Menampilkan cara bekerja dengan koleksi sumber daya.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// tambahkan sumber daya kosong
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// tambahkan sumber daya dengan nama
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// tambahkan sumber daya sebelum sumber daya dengan ID yang ditentukan
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// dapatkan sumber daya berdasarkan id
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// koleksi sumber daya tidak mendukung operasi Clear
// project.Resources.Clear();
// gunakan contoh kode berikutnya sebagai gantinya
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Lihat Juga

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


