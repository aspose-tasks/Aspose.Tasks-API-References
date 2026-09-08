---
title: "Klasse BaselineCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.BaselineCollection‑klasse. Vertegenwoordigt een verzameling van Baseline‑objecten"
type: docs
weight: 120
url: /nl/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Vertegenwoordigt een verzameling van [`Baseline`](../baseline/) objecten.

```csharp
public class BaselineCollection : IList<Baseline>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Haalt het aantal objecten op dat in dit BaselineCollection‑object is opgenomen. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Retourneert het element op de opgegeven index. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Haalt de bovenliggende [`Resource`](../resource/) voor deze verzameling op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Dit is de stub-implementatie van de Add-methode van ICollection, die alleen NotSupportedException gooit. |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Verwijdert de baseline uit deze collectie. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Converteert het BaselineCollection‑object naar een lijst van [`Baseline`](../baseline/) objecten. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


