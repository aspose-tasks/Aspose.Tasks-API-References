---
title: "Rsc.Cost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. التكلفة الإجمالية المجدولة أو المتوقعة لمورد بناءً على التكاليف التي تم تكبدها بالفعل للعمل المنفذ من قبل الموارد المخصصة للمهام بالإضافة إلى التكاليف المخططة للعمل المتبقي"
type: docs
weight: 220
url: /ar/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

التكلفة المجدولة أو المتوقعة الإجمالية لمورد، بناءً على التكاليف التي تم تكبدها بالفعل للعمل الذي قام به الموارد المعينة للمهام، بالإضافة إلى التكاليف المخطط لها للعمل المتبقي.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


