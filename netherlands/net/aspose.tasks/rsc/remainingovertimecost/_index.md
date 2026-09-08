---
title: "Rsc.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De resterende geplande overurenkosten voor een resource."
type: docs
weight: 590
url: /nl/net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

De resterende geplande overurenkosten voor een resource.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.RemainingOvertimeCost te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


