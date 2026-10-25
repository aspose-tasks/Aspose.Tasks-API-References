---
title: "Calendar.MakeNightShiftCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تجعل Calendar معينًا كNight Shift Calendar"
type: docs
weight: 20
url: /ar/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

يجعل التقويم المحدد تقويمًا للوردية الليلية.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| تقويم | Calendar | Calendar لإنشاء Night Shift Calendar. |

### قيمة الإرجاع

Night Shift Calendar.

## الأمثلة

يظهر كيفية إنشاء تقويم نوبة ليلية.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// عرض ساعات العمل
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

يظهر كيفية تحويل تقويم إلى تقويم نوبة ليلية.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// عرض ساعات العمل
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


