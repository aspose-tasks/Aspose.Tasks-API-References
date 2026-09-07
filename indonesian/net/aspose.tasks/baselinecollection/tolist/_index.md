---
title: "BaselineCollection.ToList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode BaselineCollection. Mengonversi objek BaselineCollection menjadi daftar objek Baseline"
type: docs
weight: 70
url: /id/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Mengonversi objek BaselineCollection menjadi daftar objek [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### Nilai Kembali

Daftar objek [`Baseline`](../../baseline/).

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


