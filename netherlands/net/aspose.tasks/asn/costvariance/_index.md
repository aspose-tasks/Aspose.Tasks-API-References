---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. Het verschil tussen de baselinekosten en de totale kosten voor een toewijzing"
type: docs
weight: 200
url: /nl/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

Het verschil tussen de basislijnkosten en de totale kosten voor een opdracht.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


