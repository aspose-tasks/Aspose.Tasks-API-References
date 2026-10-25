---
title: "Asn.StartVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. الفارق في تاريخ بدء التعيين عن تاريخ البدء الأساسي"
type: docs
weight: 510
url: /ar/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

الانحراف في تاريخ بدء المهمة عن تاريخ البدء الأساسي.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


