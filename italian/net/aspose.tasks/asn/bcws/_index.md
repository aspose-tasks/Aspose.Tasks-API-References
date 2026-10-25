---
title: "Asn.BCWS"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Il costo preventivato di un lavoro sull'assegnazione"
type: docs
weight: 130
url: /it/net/aspose.tasks/asn/bcws/
---
## Asn.BCWS field

Il costo preventivato del lavoro sull'assegnazione.

```csharp
public static readonly Key<double, AsnKey> BCWS;
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


