---
title: "BaselineCollection.ParentResource"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà BaselineCollection. Ottiene la Resource genitore per questa collezione"
type: docs
weight: 30
url: /it/net/aspose.tasks/baselinecollection/parentresource/
---
## BaselineCollection.ParentResource property

Ottiene la [`Resource`](../../resource/) genitore per questa collezione.

```csharp
public Resource ParentResource { get; }
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

* class [Resource](../../resource/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


