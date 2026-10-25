---
title: "Rsc.OvertimeRateFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي"
type: docs
weight: 520
url: /ar/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

الوحدات التي يستخدمها Microsoft Project لعرض معدل العمل الإضافي.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


