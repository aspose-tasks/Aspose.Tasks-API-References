---
title: "Asn.RemainingCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. Il costo previsto residuo per completare un'assegnazione"
type: docs
weight: 430
url: /it/net/aspose.tasks/asn/remainingcost/
---
## Asn.RemainingCost field

Il costo previsto rimanente per completare un'assegnazione.

```csharp
public static readonly Key<decimal, AsnKey> RemainingCost;
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


