---
title: "Asn.CostVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atama için temel maliyet ile toplam maliyet arasındaki fark"
type: docs
weight: 200
url: /tr/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

Bir atama için temel maliyet ile toplam maliyet arasındaki fark.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## Örnekler

Atamanın varyanslarını nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Atama varyanslarını yazdır
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


