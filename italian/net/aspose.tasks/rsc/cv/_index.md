---
title: "Rsc.CV"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La varianza del costo del valore guadagnato fino alla data di stato del progetto. CV è la differenza tra il BCWP (costo di lavoro previsto) del compito e l'ACWP (costo di lavoro effettivo)"
type: docs
weight: 270
url: /it/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

La varianza di costo del valore guadagnato, fino alla data di stato del progetto. CV è la differenza tra il BCWP (costo preventivato del lavoro eseguito) e l'ACWP (costo effettivo del lavoro eseguito) dell'attività.

```csharp
public static readonly Key<double, RscKey> CV;
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


