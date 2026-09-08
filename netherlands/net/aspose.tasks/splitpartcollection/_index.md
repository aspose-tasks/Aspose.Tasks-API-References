---
title: "Klasse SplitPartCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.SplitPartCollection klasse. Collectie die de delen van een taak vertegenwoordigt."
type: docs
weight: 2300
url: /nl/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Collectie die de delen van een taak voorstelt.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Haalt het aantal delen in de collectie op. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Haal een gesplitst deel van een taak op op de opgegeven index. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Kopieert alle delen van de collectie naar een nieuwe array. |

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

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


