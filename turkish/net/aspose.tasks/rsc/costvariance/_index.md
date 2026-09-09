---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak için temel maliyet ile toplam maliyet arasındaki fark"
type: docs
weight: 250
url: /tr/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

Bir kaynak için temel maliyet ile toplam maliyet arasındaki fark.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Örnekler

Rsc.CostVariance özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


