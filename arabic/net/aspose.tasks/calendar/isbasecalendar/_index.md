---
title: "Calendar.IsBaseCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Calendar. تحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا"
type: docs
weight: 70
url: /ar/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

يحصل على قيمة تشير إلى ما إذا كان التقويم تقويمًا أساسيًا.

```csharp
public bool IsBaseCalendar { get; }
```

## الأمثلة

يظهر كيفية قراءة تقويمات المشروع وخصائصها.

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // إظهار ما إذا كان لديه تقويم أساسي
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // احصل على الوقت بالساعات لكل يوم عمل
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


