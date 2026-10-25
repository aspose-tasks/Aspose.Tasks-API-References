---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc veld. Het verschil tussen de basiskost en de totale kost voor een resource"
type: docs
weight: 250
url: /nl/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

Het verschil tussen de baseline-kosten en de totale kosten voor een resource.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Voorbeelden

Toont hoe de eigenschap Rsc.CostVariance te lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


