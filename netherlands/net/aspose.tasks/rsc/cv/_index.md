---
title: "Rsc.CV"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De verdiende-waarde kostvariantie tot de projectstatusdatum. CV is het verschil tussen de BCWP (budgeted cost of work performed) en de ACWP (actual cost of work performed) van de taken."
type: docs
weight: 270
url: /nl/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

De earned value kostenvariantie tot de projectstatusdatum. CV is het verschil tussen de BCWP (begrote kosten van uitgevoerd werk) en de ACWP (werkelijke kosten van uitgevoerd werk) van de taak.

```csharp
public static readonly Key<double, RscKey> CV;
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


