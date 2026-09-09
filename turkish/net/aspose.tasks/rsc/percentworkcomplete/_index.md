---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Rsc alanı. Tüm görevlerde tamamlanan işin yüzdesi"
type: docs
weight: 550
url: /tr/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Tüm görevlerde tamamlanan iş yüzdesi.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Örnekler

Kaynak yüzde iş tamamlamasının nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Tüm kaynaklar için iş yüzde tamamlama görüntüsü
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


