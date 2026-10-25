---
title: "Asn.RemainingOvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. العمل الإضافي المتبقي المجدول لإكمال تكليف"
type: docs
weight: 450
url: /ar/net/aspose.tasks/asn/remainingovertimework/
---
## Asn.RemainingOvertimeWork field

العمل الإضافي المتبقي المجدول لإكمال مهمة.

```csharp
public static readonly Key<Duration, AsnKey> RemainingOvertimeWork;
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


