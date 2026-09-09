---
title: "Rsc.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Microsoft Project tarafından fazla mesai oranını görüntülemek için kullanılan birimler."
type: docs
weight: 520
url: /tr/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimler.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


