---
title: "Asn.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De resterende geprojecteerde overurenkosten voor het voltooien van een toewijzing"
type: docs
weight: 440
url: /nl/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

De resterende geraamde overurenkosten voor het voltooien van een toewijzing.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
```

## Voorbeelden

Toont hoe overuren/resterende werkzaamheden/kosten van een toewijzing gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Print overuren van de toewijzing
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


