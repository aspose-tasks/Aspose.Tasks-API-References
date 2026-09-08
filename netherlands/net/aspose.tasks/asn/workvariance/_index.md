---
title: "Asn.WorkVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. Het verschil tussen het baseline-werk van een taak en het momenteel geplande werk"
type: docs
weight: 620
url: /nl/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

Het verschil tussen de baseline-werk van een taak en het momenteel geplande werk.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


