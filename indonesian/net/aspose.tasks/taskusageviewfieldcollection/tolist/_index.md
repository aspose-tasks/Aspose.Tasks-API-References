---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskUsageViewFieldCollection. Mengembalikan daftar yang berisi semua item dari koleksi ini"
type: docs
weight: 20
url: /id/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Mengembalikan daftar yang berisi semua item dari koleksi ini.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Nilai Kembali

mengembalikan daftar yang berisi semua item dari koleksi ini.

## Contoh

Menampilkan cara bekerja dengan koleksi bidang dari sebuah instance TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Anda dapat mengubah koleksi menjadi daftar TaskUsageViewField
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Lihat Juga

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


