---
title: "Asn.CostVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La differenza tra il costo di baseline e il costo totale per un'assegnazione"
type: docs
weight: 200
url: /it/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

La differenza tra il costo di base e il costo totale per un'assegnazione.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## Esempi

Mostra come leggere le varianze dell'assegnazione.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Stampa le varianze dell'assegnazione
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


