---
title: "Asn.StartVariance"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamanın başlangıç tarihinin temel başlangıç tarihinden sapması"
type: docs
weight: 510
url: /tr/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

Bir atama başlangıç tarihinin temel başlangıç tarihinden sapması.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


