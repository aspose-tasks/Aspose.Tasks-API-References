---
title: "Rsc.Cost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Görevlerde atanan kaynaklar tarafından gerçekleştirilen iş için zaten oluşmuş maliyetler ve kalan iş için planlanan maliyetler dahil olmak üzere, bir kaynak için toplam planlanmış veya öngörülen maliyet"
type: docs
weight: 220
url: /tr/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Görevlere atanan kaynaklar tarafından yapılan iş için zaten oluşmuş maliyetler ve kalan iş için planlanan maliyetler temel alınarak bir kaynak için toplam planlanmış veya tahmini maliyet.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


