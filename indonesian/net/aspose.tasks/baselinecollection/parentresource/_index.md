---
title: "BaselineCollection.ParentResource"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti BaselineCollection. Mendapatkan Resource induk untuk koleksi ini"
type: docs
weight: 30
url: /id/net/aspose.tasks/baselinecollection/parentresource/
---
## BaselineCollection.ParentResource property

Mendapatkan [`Resource`](../../resource/) induk untuk koleksi ini.

```csharp
public Resource ParentResource { get; }
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

* class [Resource](../../resource/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


