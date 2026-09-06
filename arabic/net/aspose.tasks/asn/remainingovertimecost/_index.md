---
title: "Asn.RemainingOvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. التكلفة المتبقية المتوقعة للعمل الإضافي لإكمال تعيين"
type: docs
weight: 440
url: /ar/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

تكلفة العمل الإضافي المتوقعة المتبقية لإكمال مهمة.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
```

## الأمثلة

يظهر كيفية قراءة العمل الإضافي/الأعمال المتبقية/التكاليف لتكليف.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// طباعة العمل الإضافي للتكليف
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

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


