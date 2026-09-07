---
title: "Asn.CV"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La varianza di costo del valore guadagnato. CV è la differenza tra il BCWP (costo preventivato del lavoro eseguito) dell'assegnazione e l'ACWP (costo reale del lavoro eseguito)."
type: docs
weight: 220
url: /it/net/aspose.tasks/asn/cv/
---
## Asn.CV field

La varianza del costo del valore guadagnato. CV è la differenza tra il BCWP (costo preventivato del lavoro eseguito) dell'assegnazione e l'ACWP (costo effettivo del lavoro eseguito).

```csharp
public static readonly Key<double, AsnKey> CV;
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


