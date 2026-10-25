---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De hoeveelheid werk die op een toewijzing is voltooid"
type: docs
weight: 400
url: /nl/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

De hoeveelheid werk die op een toewijzing is voltooid.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Voorbeelden

Toont hoe het percentage voltooid werk van een toewijzing te lezen.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Print voltooiingspercentage van een toewijzing
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


