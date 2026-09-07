---
title: "Kelas ResourceCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ResourceCollection. Mewakili kumpulan objek Resource"
type: docs
weight: 1770
url: /id/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Mewakili kumpulan objek [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam ResourceCollection. Int32 hanya-baca. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Mendapatkan proyek induk dari objek ResourceCollection. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Menambahkan sumber daya baru pada posisi terakhir dalam koleksi sumber daya proyek. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Menambahkan sumber daya baru pada posisi terakhir dalam koleksi sumber daya proyek. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Menambahkan sumber daya baru pada posisi yang ditentukan dalam koleksi sumber daya proyek. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Penghapusan langsung tidak didukung, metode ini hanya melempar NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Mengembalikan sumber daya dengan id yang ditentukan. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Mengembalikan sumber daya dengan Uid yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Ini adalah implementasi stub dari metode Remove milik ICollection, yang hanya melempar NotSupportedException |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Mengonversi objek ResourceCollection menjadi daftar objek [`Resource`](../resource/). |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


