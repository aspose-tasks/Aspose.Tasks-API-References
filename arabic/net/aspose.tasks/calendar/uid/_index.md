---
title: "Calendar.Uid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. يحصل أو يحدد المعرف الفريد للتقويم"
type: docs
weight: 110
url: /ar/net/aspose.tasks/calendar/uid/
---
## Calendar.Uid property

يحصل أو يعيّن المعرف الفريد للتقويم.

```csharp
public int Uid { get; set; }
```

## الأمثلة

يعرض كيفية استرجاع معلومات التقويم.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// استرجاع معلومات التقويمات
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


