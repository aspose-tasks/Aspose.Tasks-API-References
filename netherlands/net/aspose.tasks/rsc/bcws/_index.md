---
title: "Rsc.BCWS"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De begrote kostprijs van werk dat voor een resource is gepland."
type: docs
weight: 150
url: /nl/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

De begrote kosten van een werk gepland voor een resource.

```csharp
public static readonly Key<double, RscKey> BCWS;
```

## Voorbeelden

Toont hoe resourcekosten te lezen.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Alle resourcekosten weergeven.
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


