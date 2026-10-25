---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceUsageViewFieldCollection. Mengonversi instance dari kelas ResourceUsageViewFieldCollection menjadi daftar yang berisi instance dari kelas ResourceUsageViewField"
type: docs
weight: 20
url: /id/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Mengonversi instance dari kelas [`ResourceUsageViewFieldCollection`](../) menjadi daftar yang berisi instance dari kelas [`ResourceUsageViewField`](../../resourceusageviewfield/)

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Nilai Kembali

Instance dari kelas [`ResourceUsageViewFieldCollection`](../) yang dikonversi menjadi daftar yang berisi instance dari kelas [`ResourceUsageViewField`](../../resourceusageviewfield/)

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

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


