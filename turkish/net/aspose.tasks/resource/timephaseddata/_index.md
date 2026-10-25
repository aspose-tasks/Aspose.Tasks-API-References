---
title: "Resource.TimephasedData"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Bu nesne için TimephasedDataCollection sınıfının bir örneğini alır veya ayarlar"
type: docs
weight: 740
url: /tr/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Bu nesne için bir [`TimephasedDataCollection`](../../timephaseddatacollection/) sınıfının örneğini alır veya ayarlar.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Açıklamalar

Okuma yalnızca XML biçimi için desteklenir.

## Örnekler

Kaynak zaman aşamalı verilerini nasıl okuyacağınızı gösterir.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// kaynağın zaman aşamalı verileri üzerinde yineleme yapın
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### Ayrıca Bakınız

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


