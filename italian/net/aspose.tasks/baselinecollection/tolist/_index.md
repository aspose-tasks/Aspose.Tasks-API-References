---
title: "BaselineCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "BaselineCollection metodo. Converte l'oggetto BaselineCollection in un elenco di oggetti Baseline"
type: docs
weight: 70
url: /it/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Converte l'oggetto BaselineCollection in un elenco di oggetti [`Baseline`](../../baseline/).

```csharp
public List<Baseline> ToList()
```

### Valore di ritorno

Elenco di oggetti [`Baseline`](../../baseline/).

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


