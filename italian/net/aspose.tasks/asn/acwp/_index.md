---
title: "Asn.ACWP"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Il costo effettivo del lavoro eseguito su un'assegnazione fino ad oggi"
type: docs
weight: 90
url: /it/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

Il costo effettivo di un lavoro eseguito su un'assegnazione fino ad oggi.

```csharp
public static readonly Key<double, AsnKey> ACWP;
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


