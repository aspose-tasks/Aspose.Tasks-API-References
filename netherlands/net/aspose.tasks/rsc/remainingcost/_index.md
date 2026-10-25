---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. De resterende geplande uitgave die zal worden gemaakt bij het voltooien van het resterende geplande werk"
type: docs
weight: 580
url: /nl/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

De resterende geplande kosten die gemaakt zullen worden bij het voltooien van het resterende geplande werk.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.RemainingCost te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


