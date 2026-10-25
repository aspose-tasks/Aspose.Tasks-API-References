---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Kosten gemaakt voor overuren die al zijn uitgevoerd op taken door toegewezen resources"
type: docs
weight: 40
url: /nl/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Kosten die zijn gemaakt voor overwerk dat al op taken door toegewezen resources is uitgevoerd.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.ActualOvertimeCost te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


