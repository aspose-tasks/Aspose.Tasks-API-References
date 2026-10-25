---
title: "Rsc.SV"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Proje durum tarihine kadar kazanılmış değer zaman çizelgesi sapması. SV, gerçekleşen işin bütçelenen maliyeti (BCWP) ile planlanan işin bütçelenen maliyeti (BCWS) arasındaki farktır."
type: docs
weight: 650
url: /tr/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

Proje durum tarihine kadar kazanılan değer zaman sapması. SV, gerçekleştirilen işin bütçelenen maliyeti (BCWP) ile planlanan işin bütçelenen maliyeti (BCWS) arasındaki farktır.

```csharp
public static readonly Key<double, RscKey> SV;
```

## Örnekler

Kaynak maliyetlerini nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Tüm kaynak maliyetlerini göster
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


