---
title: "Asn.CostVariance"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Asn. الفرق بين تكلفة الخط الأساسي وإجمالي التكلفة لتعيين"
type: docs
weight: 200
url: /ar/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

الفرق بين تكلفة الأساس والتكلفة الإجمالية للمهمة.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


