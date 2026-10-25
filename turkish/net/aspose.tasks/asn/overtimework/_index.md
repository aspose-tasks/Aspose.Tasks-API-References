---
title: "Asn.OvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamanın planlanan fazla mesai çalışması"
type: docs
weight: 380
url: /tr/net/aspose.tasks/asn/overtimework/
---
## Asn.OvertimeWork field

Bir atamanın planlanan fazla mesai işi.

```csharp
public static readonly Key<Duration, AsnKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


