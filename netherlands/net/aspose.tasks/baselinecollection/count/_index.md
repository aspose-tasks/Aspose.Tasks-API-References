---
title: "BaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "BaselineCollection eigenschap. Haalt het aantal objecten op dat in dit BaselineCollection-object is opgenomen"
type: docs
weight: 10
url: /nl/net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

Haalt het aantal objecten op dat in dit BaselineCollection‑object is opgenomen.

```csharp
public int Count { get; }
```

## Voorbeelden

Toont hoe je met baseline‑verzamelingen werkt.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// lees baseline‑informatie
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

### Zie ook

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


