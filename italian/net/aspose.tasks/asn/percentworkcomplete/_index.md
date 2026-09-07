---
title: "Asn.PercentWorkComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La quantità di lavoro completato su un'assegnazione"
type: docs
weight: 400
url: /it/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

La quantità di lavoro completato su un'assegnazione.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Esempi

Mostra come leggere la percentuale di lavoro completato di un'assegnazione.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Stampa la percentuale di completamento dell'assegnazione
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


