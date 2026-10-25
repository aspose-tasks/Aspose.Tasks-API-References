---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPartCollection methode. Kopieert alle delen van de collectie naar een nieuwe array."
type: docs
weight: 40
url: /nl/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Kopieert alle delen van de collectie naar een nieuwe array.

```csharp
public SplitPart[] ToArray()
```

### Retourwaarde

Een array van [`SplitPart`](../../splitpart/) objecten.

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


