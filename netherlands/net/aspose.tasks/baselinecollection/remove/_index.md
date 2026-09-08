---
title: "BaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "BaselineCollection methode. Verwijdert baseline uit deze collectie"
type: docs
weight: 60
url: /nl/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Verwijdert de baseline uit deze collectie.

```csharp
public bool Remove(Baseline item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | Baseline | Het item om te verwijderen. |

### Retourwaarde

true als de [`Baseline`](../../baseline/) instantie succesvol is verwijderd; anders, false

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


