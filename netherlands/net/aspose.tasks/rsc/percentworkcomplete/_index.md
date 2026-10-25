---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Het percentage voltooid werk over alle taken"
type: docs
weight: 550
url: /nl/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Het percentage van het voltooide werk over alle taken.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Voorbeelden

Toont hoe het percentage voltooid werk van een resource gelezen kan worden.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Toon de voltooiingspercentage van werk voor alle resources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


