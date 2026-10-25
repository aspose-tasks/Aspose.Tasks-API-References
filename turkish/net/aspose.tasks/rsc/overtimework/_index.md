---
title: "Rsc.OvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Bir kaynağın bir görevde gerçekleştirmesi planlanan fazla mesainin miktarı ve ilgili kaynakların fazla mesai oranlarıyla ücretlendirilir"
type: docs
weight: 530
url: /tr/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

Bir kaynağın bir görevde yapması planlanan ve ilgili kaynakların fazla mesai oranlarıyla ücretlendirilen fazla mesai miktarı.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


