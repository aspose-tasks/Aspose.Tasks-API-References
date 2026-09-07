---
title: "Kelas ResourceUsageViewFieldCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ResourceUsageViewFieldCollection. Mewakili kumpulan nilai ResourceUsageViewField"
type: docs
weight: 1830
url: /id/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Mewakili kumpulan nilai [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Mengonversi instance kelas `ResourceUsageViewFieldCollection` menjadi daftar yang berisi instance kelas [`ResourceUsageViewField`](../resourceusageviewfield/). |

## Contoh

Menampilkan cara bekerja dengan koleksi bidang dari sebuah instance ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Anda dapat mengubah koleksi menjadi daftar ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Lihat Juga

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


