---
title: "Rsc.CV"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Proje durum tarihine kadar elde edilen değer maliyet varyansı. CV, görevlerin BCWP (bütçelenen gerçekleşen iş maliyeti) ile ACWP (gerçekleşen işin gerçek maliyeti) arasındaki farktır."
type: docs
weight: 270
url: /tr/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

Proje durum tarihine kadar elde edilen değer maliyet sapması. CV, görevin BCWP'si (gerçekleştirilen işin bütçelenen maliyeti) ile ACWP'si (gerçekleştirilen işin gerçek maliyeti) arasındaki farktır.

```csharp
public static readonly Key<double, RscKey> CV;
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


