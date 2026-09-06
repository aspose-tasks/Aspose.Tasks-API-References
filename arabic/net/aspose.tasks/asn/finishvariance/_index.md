---
title: "Asn.FinishVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. الفارق بين تاريخ انتهاء التعيين وتاريخ الانتهاء الأساسي"
type: docs
weight: 250
url: /ar/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

الانحراف في تاريخ انتهاء المهمة عن تاريخ الانتهاء الأساسي.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
```

## الأمثلة

يعرض كيفية قراءة فروق التعيين.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// طباعة فروق التعيين
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


