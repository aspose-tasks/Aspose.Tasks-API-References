---
title: "Asn.SV"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La varianza di programmazione del valore guadagnato fino alla data di stato del progetto. La varianza di programmazione SV è la differenza tra BCWP e BCWS"
type: docs
weight: 540
url: /it/net/aspose.tasks/asn/sv/
---
## Asn.SV field

La varianza di programma del valore guadagnato, fino alla data di stato del progetto. La varianza di programma (SV) è la differenza tra BCWP e BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
```

## Esempi

Mostra come leggere i valori di costo dell'assegnazione.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Stampa i costi di assegnazione delle risorse
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


