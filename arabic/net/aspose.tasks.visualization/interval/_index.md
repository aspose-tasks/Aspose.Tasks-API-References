---
title: "التعداد Interval"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.Interval. يحدد الفواصل المتكررة لعرض خطوط التقدم عند"
type: docs
weight: 3170
url: /ar/net/aspose.tasks.visualization/interval/
---
## Interval enumeration

يحدد الفواصل المتكررة لعرض خطوط التقدم عندها.

```csharp
public enum Interval
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Daily | `0` | يشير إلى الفاصل اليومي. |
| Weekly | `1` | يشير إلى الفاصل الأسبوعي. |
| Monthly | `2` | يشير إلى الفاصل الشهري. |

## الأمثلة

يوضح كيفية العمل مع الفاصل المتكرر لخطوط التقدم.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// يسمح بقراءة خط التقدم
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// يسمح بإعادة تعريف الفاصل المتكرر
var newInterval = new RecurringInterval();

// تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم الشهرية حسب اليوم.
interval.MonthlyDay = true;
// تعيين رقم اليوم لخطوط التقدم الشهرية.
interval.MonthlyDayDayNumber = 1;
// تعيين رقم الشهر لخطوط التقدم الشهرية.
interval.MonthlyDayMonthNumber = 1;
// تعيين قيمة تشير إلى ما إذا كان سيتم عرض خطوط التقدم حسب اليوم الأول أو الأخير المحدد مسبقًا.
interval.MonthlyFirstLast = true;
// تعيين نوع اليوم الأول أو الأخير لخطوط التقدم الشهرية.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// تعيين رقم الشهر لخطوط التقدم التي تُعرض حسب اليوم الأول أو الأخير المحدد مسبقًا.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


