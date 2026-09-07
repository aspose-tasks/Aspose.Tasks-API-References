---
title: "Rsc.Cost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il costo totale programmato o previsto per una risorsa basato sui costi già sostenuti per il lavoro svolto dalle risorse assegnate alle attività, oltre ai costi pianificati per il lavoro rimanente"
type: docs
weight: 220
url: /it/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Il costo totale programmato o previsto per una risorsa, basato sui costi già sostenuti per il lavoro eseguito dalle risorse assegnate alle attività, oltre ai costi pianificati per il lavoro rimanente.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


