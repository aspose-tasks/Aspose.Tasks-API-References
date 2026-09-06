---
title: "Rsc.ACWP"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التكلفة الفعلية للعمل الذي قام به مورد للمشروع حتى الآن"
type: docs
weight: 90
url: /ar/net/aspose.tasks/rsc/acwp/
---
## Rsc.ACWP field

التكلفة الفعلية للعمل الذي قام به مورد للمشروع حتى الآن.

```csharp
public static readonly Key<double, RscKey> ACWP;
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


