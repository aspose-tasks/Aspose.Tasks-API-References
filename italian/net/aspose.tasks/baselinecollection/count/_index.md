---
title: "BaselineCollection.Count"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "BaselineCollection proprietà. Ottiene il numero di oggetti contenuti in questo oggetto BaselineCollection"
type: docs
weight: 10
url: /it/net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

Ottiene il numero di oggetti contenuti in questo oggetto BaselineCollection.

```csharp
public int Count { get; }
```

## Esempi

Mostra come lavorare con le collezioni di baseline.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// leggi le informazioni di baseline
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

### Vedi anche

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


