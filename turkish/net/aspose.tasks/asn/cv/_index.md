---
title: "Asn.CV"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Kazanılan değer maliyet sapması. CV, atamanın BCWP (bütçelenen gerçekleştirilen iş maliyeti) ile ACWP (gerçekleşen iş maliyeti) arasındaki farktır"
type: docs
weight: 220
url: /tr/net/aspose.tasks/asn/cv/
---
## Asn.CV field

Kazanılmış değer maliyet sapması. CV, atamanın BCWP (gerçekleştirilen işin bütçelenen maliyeti) ve ACWP (gerçekleştirilen işin gerçek maliyeti) arasındaki farktır.

```csharp
public static readonly Key<double, AsnKey> CV;
```

## Örnekler

Atamanın maliyet değerlerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Kaynak atama maliyetlerini yazdır
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


