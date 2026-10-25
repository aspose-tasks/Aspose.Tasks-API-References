---
title: "Resource.Baselines"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-eigenschap. Haalt een BaselineCollection‑instantie op voor dit object. De baseline‑waarden voor een resource"
type: docs
weight: 160
url: /nl/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Haalt een BaselineCollection‑instantie op voor dit object. De basislijnwaarden voor een resource.

```csharp
public BaselineCollection Baselines { get; }
```

## Voorbeelden

Toont hoe de baselines van een resource gelezen kunnen worden.

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

### Zie ook

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


