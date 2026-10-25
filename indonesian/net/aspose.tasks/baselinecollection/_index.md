---
title: "Kelas BaselineCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.BaselineCollection. Mewakili kumpulan objek Baseline."
type: docs
weight: 120
url: /id/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Mewakili kumpulan objek [`Baseline`](../baseline/) .

```csharp
public class BaselineCollection : IList<Baseline>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Mendapatkan jumlah objek yang terkandung dalam objek BaselineCollection ini. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Mendapatkan [`Resource`](../resource/) induk untuk koleksi ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Menghapus baseline dari koleksi ini. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Mengonversi objek BaselineCollection menjadi daftar objek [`Baseline`](../baseline/) . |

## Contoh

Menampilkan cara bekerja dengan koleksi baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// baca informasi baseline
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### Lihat Juga

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


