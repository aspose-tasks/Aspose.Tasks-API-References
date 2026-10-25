---
title: "Asn.Stop"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Atamanın durdurulduğu tarih"
type: docs
weight: 520
url: /tr/net/aspose.tasks/asn/stop/
---
## Asn.Stop field

Atamanın durdurulduğu tarih.

```csharp
public static readonly Key<DateTime, AsnKey> Stop;
```

## Örnekler

Atamanın durdurma/yeniden başlatma tarihlerini okuma nasıl gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Kaynak atamanın durdurma ve yeniden başlatma tarihlerini yazdır
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


