---
title: "BaselineCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti BaselineCollection. Mendapatkan jumlah objek yang terdapat dalam objek BaselineCollection ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

Mendapatkan jumlah objek yang terkandung dalam objek BaselineCollection ini.

```csharp
public int Count { get; }
```

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

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


