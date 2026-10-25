---
title: "Asn.OvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. العمل الإضافي المجدول لتعيين"
type: docs
weight: 380
url: /ar/net/aspose.tasks/asn/overtimework/
---
## Asn.OvertimeWork field

العمل الإضافي المجدول للمهمة.

```csharp
public static readonly Key<Duration, AsnKey> OvertimeWork;
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


