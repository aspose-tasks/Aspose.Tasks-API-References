---
title: "Asn.FinishVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La variazione della data di fine dell'assegnazione rispetto alla data di fine di baseline"
type: docs
weight: 250
url: /it/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

La varianza della data di fine di un'assegnazione rispetto a una data di fine di base.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


