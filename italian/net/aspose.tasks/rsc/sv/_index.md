---
title: "Rsc.SV"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La varianza di programmazione del valore guadagnato fino alla data di stato del progetto. SV è la differenza tra il costo preventivato del lavoro eseguito (BCWP) e il costo preventivato del lavoro programmato (BCWS)"
type: docs
weight: 650
url: /it/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

La varianza di programma del valore guadagnato, fino alla data di stato del progetto. SV è la differenza tra il costo preventivato del lavoro eseguito (BCWP) e il costo preventivato del lavoro programmato (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


