---
title: "Calendar.GetNextWorkingDayStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تحسب بداية يوم العمل التالي للتاريخ المحدد"
type: docs
weight: 180
url: /ar/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

يحسب بداية يوم العمل التالي للتاريخ المحدد.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| التاريخ | DateTime | التاريخ الذي يُحسب له بداية اليوم العامل التالي. |

### قيمة الإرجاع

تاريخ ووقت بداية اليوم العامل التالي.

## الأمثلة

يوضح كيفية الحصول على بداية يوم العمل التالي باستخدام التقويم.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// احصل على بداية يوم العمل التالي (يتم تخطي عطلة نهاية الأسبوع)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// سيتم طباعة 13 أبريل 2020 9:00 ص
Console.WriteLine(nextWorkingDayStart);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


