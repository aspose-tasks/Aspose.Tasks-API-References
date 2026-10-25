---
title: "Asn.Resume"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Asn. La data in cui l'assegnazione è ripresa"
type: docs
weight: 490
url: /it/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

La data in cui l'assegnazione è ripresa.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Esempi

Mostra come leggere le date di interruzione/ripresa dell'assegnazione.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Stampa le date di interruzione e ripresa dell'assegnazione della risorsa
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


