---
title: "Asn.RemainingWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. العمل المتبقي المجدول لإكمال تعيين"
type: docs
weight: 460
url: /ar/net/aspose.tasks/asn/remainingwork/
---
## Asn.RemainingWork field

العمل المتبقي المجدول لإكمال مهمة.

```csharp
public static readonly Key<Duration, AsnKey> RemainingWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


