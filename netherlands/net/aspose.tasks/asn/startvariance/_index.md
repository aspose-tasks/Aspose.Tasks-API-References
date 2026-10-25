---
title: "Asn.StartVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De afwijking van de startdatum van een toewijzing ten opzichte van een baseline-startdatum"
type: docs
weight: 510
url: /nl/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

De afwijking van de startdatum van een toewijzing ten opzichte van een basisstartdatum.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


