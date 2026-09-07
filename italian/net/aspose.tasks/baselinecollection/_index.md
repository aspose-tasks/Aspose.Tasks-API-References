---
title: "Classe BaselineCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.BaselineCollection. Rappresenta una collezione di oggetti Baseline"
type: docs
weight: 120
url: /it/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Rappresenta una collezione di oggetti [`Baseline`](../baseline/).

```csharp
public class BaselineCollection : IList<Baseline>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto BaselineCollection. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Ottiene il genitore [`Resource`](../resource/) per questa collezione. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Questa è l'implementazione stub del metodo Add di ICollection, che lancia solo NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Rimuove la baseline da questa raccolta. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Converte l'oggetto BaselineCollection in un elenco di oggetti [`Baseline`](../baseline/). |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


