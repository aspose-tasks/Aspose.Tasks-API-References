---
title: "CalendarException.GetExceptionDates"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة CalendarException. تُرجع التواريخ التي يكون فيها استثناء التقويم ساريًا"
type: docs
weight: 190
url: /ar/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

يعيد التواريخ التي ينطبق عليها استثناء التقويم.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### قيمة الإرجاع

تُرجع مجموعة من تواريخ الاستثناء التي يكون فيها استثناء التقويم ساريًا.

## الأمثلة

يظهر كيفية الحصول على التواريخ التي يكون فيها استثناء تقويم محدد فعالًا.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### انظر أيضًا

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


