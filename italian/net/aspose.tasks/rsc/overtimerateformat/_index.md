---
title: "Rsc.OvertimeRateFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Le unità usate da Microsoft Project per visualizzare il tasso di straordinario"
type: docs
weight: 520
url: /it/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Le unità utilizzate da Microsoft Project per visualizzare il tasso di straordinario.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
```

## Esempi

Mostra come leggere i valori degli straordinari della risorsa.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Visualizza i parametri relativi agli straordinari per tutte le risorse
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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


