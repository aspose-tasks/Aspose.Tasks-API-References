---
title: "Asn.WorkVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. الفرق بين عمل الخط الأساسي لمهمة والعمل المجدول حاليًا"
type: docs
weight: 620
url: /ar/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

الفرق بين العمل الأساسي للمهمة والعمل المجدول حاليًا.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


