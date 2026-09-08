---
title: "Asn.FinishVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De afwijking van de einddatum van een toewijzing ten opzichte van een basislijn-einddatum"
type: docs
weight: 250
url: /nl/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

De variantie van de einddatum van een opdracht ten opzichte van een basislijn einddatum.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
```

## Voorbeelden

Toont hoe de variaties van een toewijzing te lezen.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Print toewijzingsvariaties
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


