---
title: "ResourceCollection.Clear"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceCollection. Penghapusan langsung tidak didukung, metode ini hanya melempar NotSupportedException"
type: docs
weight: 50
url: /id/net/aspose.tasks/resourcecollection/clear/
---
## ResourceCollection.Clear method

Penghapusan langsung tidak didukung, metode ini hanya melempar NotSupportedException.

```csharp
public void Clear()
```

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

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


