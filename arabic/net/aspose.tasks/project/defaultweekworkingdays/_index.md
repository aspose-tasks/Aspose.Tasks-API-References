---
title: "Project.DefaultWeekWorkingDays"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على كائن من فئة WeekDayCollection التي تمثل مجموعة من أيام العمل الأسبوعية الافتراضية للمشروع وأوقات العمل"
type: docs
weight: 370
url: /ar/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

تحصل على كائن من فئة [`WeekDayCollection`](../../weekdaycollection/) التي تمثل مجموعة من أيام العمل الأسبوعية الافتراضية للمشروع وأوقات العمل.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### قيمة الإرجاع

الكائن من فئة [`WeekDayCollection`](../../weekdaycollection/) الذي يحتوي على قائمة من كائنات [`WeekDay`](../../weekday/).

## ملاحظات

البيانات موجودة فقط في ملفات mpp (ليس في xml).

## الأمثلة

يعرض كيفية الحصول على يوم العمل الأسبوعي الافتراضي.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### انظر أيضًا

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


