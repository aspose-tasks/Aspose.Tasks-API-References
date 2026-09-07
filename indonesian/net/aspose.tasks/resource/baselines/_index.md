---
title: "Resource.Baselines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Resource. Mendapatkan instance BaselineCollection untuk objek ini. Nilai baseline untuk sebuah resource"
type: docs
weight: 160
url: /id/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Mendapatkan instance BaselineCollection untuk objek ini. Nilai baseline untuk sebuah sumber daya.

```csharp
public BaselineCollection Baselines { get; }
```

## Contoh

Menunjukkan cara membaca baseline resource.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Lihat Juga

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


