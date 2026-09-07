---
title: "Rsc.OvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il costo totale degli straordinari per una risorsa su tutti i compiti assegnati"
type: docs
weight: 500
url: /it/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Il costo totale degli straordinari per una risorsa su tutte le attività assegnate.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
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
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


