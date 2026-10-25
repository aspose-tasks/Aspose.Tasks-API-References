---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Kosten die zijn gemaakt voor werk dat al door resources op hun taken is uitgevoerd, samen met eventuele andere geregistreerde kosten die aan de taak zijn gekoppeld"
type: docs
weight: 30
url: /nl/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Kosten die zijn gemaakt voor werk dat al door resources op hun taken is uitgevoerd, samen met eventuele andere geregistreerde kosten die aan de taak zijn gekoppeld.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualCost gelezen/geschreven kan worden.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


