---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Geeft aan aan welk kostenplaats de kosten die door de resource zijn opgelopen, moeten worden toegerekend"
type: docs
weight: 230
url: /nl/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Geeft aan aan welk kostenplaats de door de resource gemaakte kosten moeten worden toegerekend.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.CostCenter te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


