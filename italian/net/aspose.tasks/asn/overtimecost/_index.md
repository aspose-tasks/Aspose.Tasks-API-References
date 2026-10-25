---
title: "Asn.OvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La somma del costo effettivo e residuo di straordinario di un'assegnazione"
type: docs
weight: 370
url: /it/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

La somma del costo effettivo e residuo degli straordinari di un'assegnazione.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
```

## Esempi

Mostra come leggere i lavori/costi di straordinario/residui di un'assegnazione.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Stampa gli straordinari dell'assegnazione
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


