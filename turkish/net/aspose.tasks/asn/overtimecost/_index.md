---
title: "Asn.OvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamanın gerçek ve kalan fazla mesai maliyetinin toplamı"
type: docs
weight: 370
url: /tr/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

Bir atamanın gerçek ve kalan fazla mesai maliyetinin toplamı.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
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


