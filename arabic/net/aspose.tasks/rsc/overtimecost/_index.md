---
title: "Rsc.OvertimeCost"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. إجمالي تكلفة العمل الإضافي لمورد على جميع المهام المعينة"
type: docs
weight: 500
url: /ar/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

إجمالي تكلفة العمل الإضافي للمورد على جميع المهام المخصصة.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## الأمثلة

يوضح كيفية قراءة قيم العمل الإضافي للمورد.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// عرض المعلمات المتعلقة بالعمل الإضافي لجميع الموارد
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


