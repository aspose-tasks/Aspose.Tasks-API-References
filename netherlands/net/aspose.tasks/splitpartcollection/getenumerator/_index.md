---
title: "SplitPartCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPartCollection methode. Retourneert een enumerator voor deze collectie."
type: docs
weight: 30
url: /nl/net/aspose.tasks/splitpartcollection/getenumerator/
---
## SplitPartCollection.GetEnumerator method

Retourneert een enumerator voor deze collectie.

```csharp
public IEnumerator<SplitPart> GetEnumerator()
```

### Retourwaarde

een enumerator voor deze collectie.

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


