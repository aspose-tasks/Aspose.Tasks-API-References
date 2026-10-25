---
title: "Asn.ACWP"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Asn alanı. Bir atamada gerçekleştirilen işin bugüne kadar olan gerçek maliyeti"
type: docs
weight: 90
url: /tr/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

Bir atama için bugüne kadar yapılan işin gerçek maliyeti.

```csharp
public static readonly Key<double, AsnKey> ACWP;
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


