---
title: "SplitPartCollection.GetEnumerator"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo SplitPartCollection. Restituisce un enumeratore per questa collezione"
type: docs
weight: 30
url: /it/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Restituisce un enumeratore per questa collezione.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Valore di ritorno

un enumeratore per questa collezione.

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


