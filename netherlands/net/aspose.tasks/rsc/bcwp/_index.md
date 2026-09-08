---
title: "Rsc.BCWP"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De begrote kosten van een werk dat door een resource voor het project is uitgevoerd tot nu toe"
type: docs
weight: 140
url: /nl/net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

De begrote kosten van een werk uitgevoerd door een resource voor het project tot nu toe.

```csharp
public static readonly Key<double, RscKey> BCWP;
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


