---
title: "Rsc.Cost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De totale geplande of geprojecteerde kost voor een resource, gebaseerd op kosten die al zijn gemaakt voor werk uitgevoerd door resources die aan de taken zijn toegewezen, naast de kosten die gepland zijn voor het resterende werk"
type: docs
weight: 220
url: /nl/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

De totale geplande of verwachte kosten voor een resource, gebaseerd op kosten die al zijn gemaakt voor werk uitgevoerd door resources die aan de taken zijn toegewezen, naast de kosten die zijn gepland voor het resterende werk.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


