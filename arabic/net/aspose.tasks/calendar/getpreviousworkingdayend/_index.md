---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تحسب نهاية تاريخ العمل السابق من التاريخ المحدد"
type: docs
weight: 190
url: /ar/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

يحسب نهاية تاريخ العمل السابق من التاريخ المحدد.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| التاريخ | DateTime | التاريخ لحساب نهاية يوم العمل السابق. |

### قيمة الإرجاع

نهاية يوم العمل السابق.

## الأمثلة

يوضح كيفية الحصول على نهاية يوم عمل سابق باستخدام تقويم.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على نهاية يوم عمل سابق
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// سيتم طباعة 9 أبريل 2020 18:00 م
Console.WriteLine(previousWorkingDayEnd);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


