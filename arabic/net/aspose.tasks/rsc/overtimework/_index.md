---
title: "Rsc.OvertimeWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. مقدار الوقت الإضافي المجدول الذي سيؤديه مورد على مهمة ويتم احتسابه بأسعار الوقت الإضافي للموارد المشاركة"
type: docs
weight: 530
url: /ar/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

كمية العمل الإضافي المجدولة التي سيؤديها المورد على مهمة ويتم احتسابها وفق معدلات العمل الإضافي للموارد المشاركة.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


