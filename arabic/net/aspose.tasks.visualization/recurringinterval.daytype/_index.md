---
title: "تعداد RecurringInterval.DayType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.RecurringIntervalDayType. يمثل نوع اليوم المستخدم في خطوط التقدم"
type: docs
weight: 3320
url: /ar/net/aspose.tasks.visualization/recurringinterval.daytype/
---
## RecurringInterval.DayType enumeration

يمثل نوع اليوم المستخدم في خطوط التقدم.

```csharp
public enum DayType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Sunday | `1` | يشير إلى الأحد. |
| Monday | `2` | يشير إلى الاثنين. |
| Tuesday | `3` | يشير إلى الثلاثاء. |
| Wednesday | `4` | يشير إلى الأربعاء. |
| Thursday | `5` | يشير إلى الخميس. |
| Friday | `6` | يشير إلى الجمعة. |
| Saturday | `7` | يشير إلى السبت. |
| Day | `8` | يشير إلى اليوم. |
| Workday | `9` | يشير إلى يوم عمل. |
| NonworkingDay | `10` | يشير إلى يوم غير عمل. |

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

* class [RecurringInterval](../recurringinterval/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


