---
title: "Rsc.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De eenheden die door Microsoft Project worden gebruikt om het overurenttarief weer te geven."
type: docs
weight: 520
url: /nl/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

De eenheden die Microsoft Project gebruikt om het overwerktarief weer te geven.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


