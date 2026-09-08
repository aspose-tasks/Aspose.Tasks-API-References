---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De totale overurenkosten voor een resource op alle toegewezen taken"
type: docs
weight: 500
url: /nl/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

De totale overurenkost voor een resource op alle toegewezen taken.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Voorbeelden

Toont hoe overurenwaarden van resources gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Toon overuren-gerelateerde parameters voor alle resources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


