---
title: "Asn.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamada tamamlanan iş miktarı"
type: docs
weight: 400
url: /tr/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

Bir atamada tamamlanan iş miktarı.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Örnekler

Bir atamanın tamamlanan iş yüzdesini nasıl okuyacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Atama yüzde tamamlamasını yazdır
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


