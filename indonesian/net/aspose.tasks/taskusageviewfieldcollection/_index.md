---
title: "Kelas TaskUsageViewFieldCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskUsageViewFieldCollection. Mewakili koleksi nilai TaskUsageViewField."
type: docs
weight: 2500
url: /id/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Mewakili koleksi nilai [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Mengembalikan daftar yang berisi semua item dari koleksi ini. |

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

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


