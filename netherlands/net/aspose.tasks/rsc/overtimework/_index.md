---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. De hoeveelheid overuren die gepland is om door een resource op een taak uitgevoerd te worden en die wordt gefactureerd tegen de overurentarieven van de betrokken resources"
type: docs
weight: 530
url: /nl/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

De hoeveelheid overwerk die is gepland voor een resource op een taak en wordt gefactureerd tegen de overwerktarieven van de betrokken resources.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


