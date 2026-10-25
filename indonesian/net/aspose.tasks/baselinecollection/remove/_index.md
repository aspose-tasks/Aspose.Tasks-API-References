---
title: "BaselineCollection.Remove"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode BaselineCollection. Menghapus baseline dari koleksi ini"
type: docs
weight: 60
url: /id/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Menghapus baseline dari koleksi ini.

```csharp
public bool Remove(Baseline item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | Baseline | Item yang akan dihapus. |

### Nilai Kembali

true jika instance [`Baseline`](../../baseline/) telah berhasil dihapus; jika tidak, false

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


