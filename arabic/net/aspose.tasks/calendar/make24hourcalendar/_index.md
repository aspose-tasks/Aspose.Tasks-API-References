---
title: "Calendar.Make24HourCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تجعل Calendar معينًا تقويمًا 24Hour Calendar. 24Hour Calendar هو Calendar يكون فيه كل يوم من أيام الأسبوع يعمل بساعات عمل مستمرة على مدار الساعة."
type: docs
weight: 10
url: /ar/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

يجعل تقويمًا معينًا تقويمًا 24 ساعة. تقويم 24 ساعة هو تقويم يعمل فيه كل يوم من الأسبوع بساعات عمل مستمرة على مدار الساعة.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| تقويم | Calendar | Calendar لإنشاء تقويم 24 ساعة من. |

### قيمة الإرجاع

تقويم 24Hour.

## الأمثلة

يوضح كيفية إنشاء تقويم 24 ساعة.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// سيتم طباعة 24 ساعة
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

يوضح كيفية تحويل تقويم جديد إلى تقويم 24 ساعة.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// سيتم طباعة 24 ساعة
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


