---
title: "Rsc.WorkVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. Het verschil tussen de basislijnwerk van een resource en het momenteel geplande werk"
type: docs
weight: 710
url: /nl/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

Het verschil tussen de baseline-werk van een resource en het momenteel geplande werk.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Voorbeelden

Toont hoe de resource-werkvariantie te lezen.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


