---
title: "SplitPartCollection.Count"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPartCollection eigenschap. Haalt het aantal delen in de collectie op."
type: docs
weight: 10
url: /nl/net/aspose.tasks/splitpartcollection/count/
---
## SplitPartCollection.Count property

Haalt het aantal delen in de collectie op.

```csharp
public int Count { get; }
```

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

* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


