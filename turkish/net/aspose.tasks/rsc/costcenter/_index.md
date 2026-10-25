---
title: "Rsc.CostCenter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Kaynak tarafından biriken maliyetlerin hangi maliyet merkezine tahsil edileceğini gösterir"
type: docs
weight: 230
url: /tr/net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Kaynak tarafından oluşan maliyetlerin hangi maliyet merkezine tahsil edileceğini gösterir.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Örnekler

Rsc.CostCenter özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


