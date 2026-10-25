---
title: "Calendar.Name"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. تحصل أو تعين اسم التقويم"
type: docs
weight: 90
url: /ar/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

يحصل أو يعيّن اسم التقويم.

```csharp
public string Name { get; set; }
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


