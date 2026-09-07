---
title: "Rsc.BCWS"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il costo di budget di un lavoro programmato per una risorsa"
type: docs
weight: 150
url: /it/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

Il costo di budget di un lavoro programmato per una risorsa.

```csharp
public static readonly Key<double, RscKey> BCWS;
```

## Esempi

Mostra come leggere i costi delle risorse.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Visualizza tutti i costi delle risorse
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

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


