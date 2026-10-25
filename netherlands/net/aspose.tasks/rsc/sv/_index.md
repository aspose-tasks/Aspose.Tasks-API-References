---
title: "Rsc.SV"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc field. De verdiende waarde schema‑variant tot de projectstatusdatum. SV is het verschil tussen begrote kosten van uitgevoerde werkzaamheden BCWP en begrote kosten van geplande werkzaamheden BCWS"
type: docs
weight: 650
url: /nl/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

De earned value-planningsvariantie tot de projectstatusdatum. SV is het verschil tussen de begrote kost van uitgevoerd werk (BCWP) en de begrote kost van gepland werk (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


