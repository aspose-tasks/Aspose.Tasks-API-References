---
title: "Rsc.OvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın tüm atanan görevlerdeki toplam fazla mesai maliyeti"
type: docs
weight: 500
url: /tr/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Kaynağın tüm atanan görevlerdeki toplam fazla mesai maliyeti.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Örnekler

Kaynak fazla mesai değerlerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Tüm kaynaklar için fazla mesai ile ilgili parametreleri göster
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


