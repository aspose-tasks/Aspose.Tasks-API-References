---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceUsageViewFieldCollection. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

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


