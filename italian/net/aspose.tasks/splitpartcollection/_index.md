---
title: "Classe SplitPartCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.SplitPartCollection. Collezione che rappresenta le parti di un'attività."
type: docs
weight: 2300
url: /it/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Collezione che rappresenta le porzioni di un'attività.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Ottiene il numero di parti nella collezione. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Recupera la parte divisa di un'attività all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Copia tutte le parti dalla collezione in un nuovo array. |

## Esempi

Mostra come lavorare con le collezioni di parti divise.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// itera sulle parti divise
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// ottieni la parte per indice
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// esegui qualche operazione con la prima parte divisa dell'attività
```

### Vedi anche

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


