---
title: "Prj.DaysPerMonth"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. عدد الأيام في الشهر"
type: docs
weight: 220
url: /ar/net/aspose.tasks/prj/dayspermonth/
---
## Prj.DaysPerMonth field

عدد الأيام في الشهر.

```csharp
public static readonly Key<int, PrjKey> DaysPerMonth;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خصائص أيام الأسبوع للمشروع.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// تعيين خصائص أيام الأسبوع
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// عرض خصائص أيام الأسبوع
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


