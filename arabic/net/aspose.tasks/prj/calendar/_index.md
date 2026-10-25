---
title: "Prj.Calendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. تقويم المشروع"
type: docs
weight: 90
url: /ar/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

تقويم المشروع.

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Prj.Calendar.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

project.Set(Prj.Calendar, calendar);

Console.WriteLine("Calendar: " + project.Get(Prj.Calendar).Name);
foreach (var weekDay in calendar.WeekDays)
{
    Console.WriteLine(weekDay.FromDate);
    Console.WriteLine(weekDay.ToDate);
}
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


