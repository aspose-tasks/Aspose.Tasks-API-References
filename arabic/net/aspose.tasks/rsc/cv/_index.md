---
title: "Rsc.CV"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. تباين تكلفة القيمة المكتسبة حتى تاريخ حالة المشروع. CV هو الفرق بين تكلفة العمل المنفذ المخطط لها (BCWP) وتكلفة العمل المنفذ الفعلية (ACWP) للمهام"
type: docs
weight: 270
url: /ar/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

انحراف تكلفة القيمة المكتسبة، حتى تاريخ حالة المشروع. CV هو الفرق بين BCWP (تكلفة العمل المنفذ المتوقعة) و ACWP (تكلفة العمل المنفذ الفعلية) للمهمة.

```csharp
public static readonly Key<double, RscKey> CV;
```

## الأمثلة

يعرض كيفية قراءة تكاليف الموارد.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// عرض جميع تكاليف الموارد
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


