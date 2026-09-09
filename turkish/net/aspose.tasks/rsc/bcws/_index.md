---
title: "Rsc.BCWS"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynak için planlanan bir işin bütçe maliyeti."
type: docs
weight: 150
url: /tr/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

Bir kaynak için planlanan işin bütçe maliyeti.

```csharp
public static readonly Key<double, RscKey> BCWS;
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


