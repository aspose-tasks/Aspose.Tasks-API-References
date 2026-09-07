---
title: "SplitPartCollection.Item"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SplitPartCollection. Recupera una parte divisa di un'attività all'indice specificato"
type: docs
weight: 20
url: /it/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Recupera la parte divisa di un'attività all'indice specificato.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice della parte. |

### Valore di ritorno

una parte divisa.

## Osservazioni

L'indice è basato su zero. Restituisce null se l'indice è al di fuori dei limiti dell'array.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


