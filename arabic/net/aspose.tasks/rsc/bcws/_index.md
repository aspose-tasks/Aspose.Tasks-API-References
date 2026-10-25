---
title: "Rsc.BCWS"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. تكلفة الميزانية لعمل مجدول لمورد"
type: docs
weight: 150
url: /ar/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

تكلفة الميزانية للعمل المجدول لمورد.

```csharp
public static readonly Key<double, RscKey> BCWS;
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


