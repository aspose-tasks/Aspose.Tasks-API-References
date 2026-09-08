---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPartCollection property. Haalt een gesplitst deel van een taak op op de opgegeven index"
type: docs
weight: 20
url: /nl/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Haal een gesplitst deel van een taak op op de opgegeven index.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parameter | Beschrijving |
| --- | --- |
| index | De onderdeelindex. |

### Retourwaarde

een gesplitst deel.

## Opmerkingen

De index is nulgebaseerd. Retourneert null als de index buiten de grenzen van de array ligt.

## Voorbeelden

Toont hoe te werken met gesplitste deelcollecties.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// itereren over gesplitste delen
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// haal het deel op op index
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// voer wat werk uit met het eerste gesplitste deel van de taak
```

### Zie ook

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


