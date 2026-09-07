---
title: "Asn.WorkVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La differenza tra il lavoro di baseline di un'attività e il lavoro attualmente programmato"
type: docs
weight: 620
url: /it/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

La differenza tra il lavoro di base di un'attività e il lavoro attualmente programmato.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


