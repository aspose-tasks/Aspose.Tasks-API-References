---
title: "Calendar.BaseCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. تحصل أو تعين التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا."
type: docs
weight: 40
url: /ar/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

يحصل أو يعيّن التقويم الأساسي الذي يعتمد عليه هذا التقويم. ينطبق فقط إذا لم يكن التقويم تقويمًا أساسيًا.

```csharp
public Calendar BaseCalendar { get; set; }
```

## الأمثلة

يظهر كيفية العمل مع تقويم أساسي لتقويم المورد.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// إضافة تقويم قياسي وتعيينه إلى المورد
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// عرض اسم التقويم الأساسي لجميع الموارد
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


