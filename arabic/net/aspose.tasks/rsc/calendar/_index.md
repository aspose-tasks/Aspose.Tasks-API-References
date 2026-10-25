---
title: "Rsc.Calendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. تقويم المورد"
type: docs
weight: 190
url: /ar/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

تقويم المورد.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## الأمثلة

يوضح كيفية الحصول على/تعيين تقويم المورد.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// إضافة تقويم قياسي وتعيينه إلى المورد
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// عرض اسم التقويم الأساسي لجميع الموارد
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


