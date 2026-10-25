---
title: "Asn.Stop"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De datum waarop de toewijzing wordt gestopt"
type: docs
weight: 520
url: /nl/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

De datum waarop de toewijzing wordt gestopt.

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
```

## Voorbeelden

Toont hoe je de stop/herstartdatums van een toewijzing kunt lezen.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Print de stop- en herstartdatums van de resource-toewijzing
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


