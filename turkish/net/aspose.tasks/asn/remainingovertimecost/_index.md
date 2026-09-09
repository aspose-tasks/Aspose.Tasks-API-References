---
title: "Asn.RemainingOvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamanın tamamlanması için kalan tahmini fazla mesai maliyeti"
type: docs
weight: 440
url: /tr/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

Bir atamayı tamamlama için kalan tahmini fazla mesai maliyeti.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
```

## Örnekler

Bir atamanın fazla mesai/kalan iş/maliyetlerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Atama fazla mesailerini yazdır
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


