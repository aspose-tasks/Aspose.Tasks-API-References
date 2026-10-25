---
title: "Rsc.OvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità di straordinario programmato da una risorsa per un'attività e addebitato alle tariffe di straordinario delle risorse coinvolte"
type: docs
weight: 530
url: /it/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

La quantità di straordinario programmata da una risorsa su un'attività e addebitata ai tassi di straordinario delle risorse coinvolte.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


