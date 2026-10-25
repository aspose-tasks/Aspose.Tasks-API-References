---
title: "WeekDay.Clone"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة WeekDay. تُرجع نسخة عميقة من يوم الأسبوع"
type: docs
weight: 80
url: /ar/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

يعيد نسخة عميقة من يوم الأسبوع.

```csharp
public WeekDay Clone()
```

### قيمة الإرجاع

تُرجع النسخة العميقة من يوم الأسبوع.

## الأمثلة

يظهر كيفية استنساخ يوم من أيام الأسبوع.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// إنشاء نسخة عميقة من يوم الأسبوع
var weekDay2 = weekDay1.Clone();

// يتم التحقق من مساواة التقويمات مقابل خصائص يوم الأسبوع:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### انظر أيضًا

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


