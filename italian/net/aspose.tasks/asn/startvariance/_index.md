---
title: "Asn.StartVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La varianza della data di inizio di un'assegnazione rispetto a una data di inizio di baseline"
type: docs
weight: 510
url: /it/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

La variazione della data di inizio di un'assegnazione rispetto a una data di inizio di baseline.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


